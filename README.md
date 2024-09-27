Chat Application

Overview

This is a real-time chat application that allows users to register, log in, and communicate with others in real time. It includes features such as sending messages, uploading images, and displaying online users. The project uses Firebase for real-time database storage and user authentication.

Features

User Authentication: Users can log in with a username and password.
Real-Time Messaging: Messages are sent and received instantly.
Image Upload: Users can upload images during the chat.
Online Users List: Displays a list of online users.
Message Editing: Users can edit previously sent messages.
Responsive Design: The layout adjusts to different screen sizes.
Demo

A live demo of the app can be run using Firebase's real-time database and hosting features. You can set up your own Firebase project to integrate with this app.

Project Structure

bash
Copy code
|-- index.html       # The login page
|-- chat.html        # The real-time chat interface
|-- script.js        # JavaScript for handling real-time messaging, Firebase integration, and app functionality
|-- login-style.css  # Styles for the login page
|-- style.css        # Styles for the chat page
index.html
The login page where users input their username and password. It checks credentials using Firebase and redirects to the chat page on successful login.

chat.html
The main chat interface shows online users and messages in real time. It allows users to send text messages, upload images, and edit messages. The page also contains modals for image viewing and message editing.

script.js
Handles all the app's interactivity, including:

Firebase initialization for database and storage.
Sending and receiving messages.
Managing user sessions and authentication.
File upload and image display.
Technologies Used

HTML5: Markup for structuring the app's interface.
CSS3: For styling the application.
JavaScript: Handling the logic for chat functionalities.
Firebase: Real-time database, user authentication, and file storage.
Font Awesome: Icons used throughout the app.
Setup Instructions

Prerequisites
You need a Firebase account to create your real-time database and storage.
Clone this repository to your local machine.
Steps:
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/chat-app.git
Install dependencies (if any additional dependencies are required).
Setup Firebase:
Go to Firebase Console.
Create a new project and enable Firebase Realtime Database and Firebase Storage.
Replace the Firebase configuration in script.js with your project details.
Run the app:
Open index.html in your browser.
Use the default login credentials:
Username: ABC
Password: Pass123
Start chatting in real-time!
Firebase Configuration

In script.js, make sure to replace the Firebase configuration with your own:

javascript
Copy code
const firebaseConfig = {

  apiKey: "YOUR_API_KEY",
  
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  
  databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
  
  projectId: "YOUR_PROJECT_ID",
  
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  
  messagingSenderId: "YOUR_SENDER_ID",
  
  appId: "YOUR_APP_ID"
};
firebase.initializeApp(firebaseConfig);
Contributing

Contributions are welcome! Feel free to open a pull request to suggest new features or improvements.
