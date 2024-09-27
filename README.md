# Chat Application

Chat Application is a real-time chat platform that allows users to register, log in, and chat with others instantly. The app supports real-time messaging, image uploads, and displays online users, making it a fully functional chat interface. Firebase powers the real-time database and user authentication.

## Features

- **User Authentication**: Register and log in with a username and password.
- **Real-Time Messaging**: Send and receive messages instantly.
- **Image Upload**: Upload and share images during the chat.
- **Online Users List**: Displays a list of currently active users.
- **Message Editing**: Users can edit previously sent messages.
- **Responsive Design**: The layout adjusts for various screen sizes.

## Demo

You can set up a live demo of the app using Firebase’s real-time database and hosting features.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/chat-app.git
    ```

2. Navigate to the project folder:
    ```bash
    cd chat-app
    ```

3. Open `index.html` in your browser to start the application.

## Configuration

- To use Firebase, replace the Firebase configuration in `script.js` with your own Firebase project details.
- Set up Firebase Realtime Database and Firebase Storage to handle the chat and file uploads.

## File Structure

|-- index.html # Login page for user authentication |-- chat.html # Main real-time chat interface |-- script.js # JavaScript for handling real-time messaging, Firebase integration |-- login-style.css # Styles for the login page |-- style.css # Styles for the chat page


## Firebase Configuration

In `script.js`, replace the Firebase configuration with your own Firebase project details:

```javascript
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

---

This version uses code block formatting (` ``` `) for markdown, making it easy to copy-paste and retain the exact format for GitHub README files.
