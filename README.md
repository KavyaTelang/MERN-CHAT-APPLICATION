# MERN CHAT APPLICATIOMN 
**COMPANY** : CODTECH IT SOLUTIONS

**NAME** : KAVYA TELANG

**INTERN ID** : CT6WKLY

**DOMAIN** : MERN STACK WEB DEVELOPMENT 

**BATCH DURATION** : January 20th, 2025 to March 5th, 2025

**MENTOR NAME** : Neela Santosh

### **Project Overview**  
The chat app includes features such as real-time messaging, user online status, and authentication. The UI is styled with Tailwind CSS and Daisy UI, and the backend is structured with a clean and modularized approach.  

### **Setting Up the Project**  
The project is divided into **frontend** and **backend** directories. The frontend is initialized using Vite for a React-based application, while the backend uses Express.js. A **package.json** file is set up in the root for better deployment management, ensuring both frontend and backend can be run together.  

### **Backend Development**  
1. **Server Setup:**  
   - Express.js is installed, along with middleware like **dotenv** for environment variables, **cookie-parser** for handling cookies, and **bcrypt.js** for password hashing.  
   - Nodemon is configured for automatic server restarts.  

2. **Authentication System:**  
   - **JWT-based Authentication:** Uses JWT tokens to manage user sessions, storing them in HTTP-only cookies.  
   - **User Signup:** New users register with a username, password, and gender. Passwords are hashed using bcrypt.js before storing in MongoDB.  
   - **User Login:** Users authenticate using their username and password. The system checks credentials and issues a JWT token.  
   - **Logout:** The server clears the JWT token from cookies to log users out.  

3. **Database Setup:**  
   - MongoDB is used with Mongoose ORM.  
   - **User Model:** Includes fields for full name, username, password, gender, and profile picture.  
   - **Message Model:** Each message consists of sender ID, receiver ID, and the message content.  
   - **Conversation Model:** Manages chat threads between users, storing participants and associated messages.  

4. **Messaging System:**  
   - Users can send and receive messages.  
   - If a conversation between two users does not exist, a new one is created.  
   - Messages are stored in MongoDB and linked to conversation threads.  
   - Messages are retrieved using Mongoose’s **populate()** method to get complete message details.  

5. **User Routes & Middleware:**  
   - A middleware function (`protectRoute`) ensures only authenticated users can send messages.  
   - A route fetches all users except the logged-in user to display on the sidebar.  

### **Frontend Development**  
1. **Setup:**  
   - React is used with Tailwind CSS and Daisy UI for styling.  
   - The frontend interacts with the backend via API calls.  

2. **User Authentication UI:**  
   - A login and signup page allow users to register and log in.  
   - The app stores JWT tokens in cookies to persist user sessions.  

3. **Real-Time Chat UI:**  
   - Messages are displayed in a chat interface.  
   - User profiles with avatars are shown in the sidebar.  

# RESOURCES - 
https://www.youtube.com/watch?v=HwCqsOis894
# OUTPUT OF TASK 
![image](https://github.com/user-attachments/assets/289be0aa-e716-42c8-bd9d-40102a4dab6d)
![image](https://github.com/user-attachments/assets/7d60b946-6bba-4913-9734-871254366709)

