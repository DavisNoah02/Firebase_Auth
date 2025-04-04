
## Firebase Authentication with React

This React application integrates **Firebase Authentication** to manage user registration, login, password reset, and Google login using Firebase. It also includes a basic Firestore setup to store user profile information.


![image](https://github.com/user-attachments/assets/4664f6c3-18c8-456b-ab91-42794a5def46)

## Features

- **User Registration** using Email/Password.
- **User Login** using Email/Password.
- **Password Reset** via email.
- **Google Sign-In** using Firebase.
- **User Profile Storage** in Firestore (Firestore Database).
- **React Toast Notifications** for success/error messages.
- **React Router** for page navigation.

## Prerequisites

- Node.js (v12 or later)
- Firebase account

## Setup Guide

### 1. Clone the Repository
Clone this project to your local machine.

```bash
git clone https://github.com/your-username/firebase-auth-react.git
cd firebase-auth-react
```

Replace `your-username` with your actual GitHub username.

### 2. Install Dependencies
Install the required dependencies using npm or yarn.

```bash
npm install
```

or

```bash
yarn install
```

### 3. Create a Firebase Project
Create a new Firebase project in the Firebase console.

### 4. Set up Firebase Configuration
Create a new file called `firebaseConfig.js` in the root of the project and add your Firebase configuration details.

```javascript
import firebase from 'firebase/app';
import 'firebase/auth';
import 'firebase/firestore';

const firebaseConfig = {
  apiKey: '<API_KEY>',
  authDomain: '<AUTH_DOMAIN>',
  databaseURL: '<DATABASE_URL>',
  projectId: '<PROJECT_ID>',
  storageBucket: '<STORAGE_BUCKET>',
  messagingSenderId: '<MESSAGING_SENDER_ID>',
};

firebase.initializeApp(firebaseConfig);

export const auth = firebase.auth();
export const db = firebase.firestore();
```

Replace the `<API_KEY>`, `<AUTH_DOMAIN>`, `<DATABASE_URL>`, `<PROJECT_ID>`, `<STORAGE_BUCKET>`, and `<MESSAGING_SENDER_ID>` placeholders with your actual Firebase configuration details.

### 5. Start the Application
Start the application using npm or yarn.

```bash
npm start
```

or

```bash
yarn start
```

The application should now be running on `http://localhost:3000`.


### 🚀 Future Improvements 🌟
```bash
1.Add a Microsoft sign-in method.

2.Implement User Roles and Permissions.

3.Add Social Logins like Facebook and Twitter.

4.Enhance security features and UI design.
```
