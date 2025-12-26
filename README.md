# Profiles Directory App

**Student Name:** Esra Özdemir  
**Student ID:** 220408014  

## Project Description
Profiles Directory App is a React Native mobile application developed using Expo.  
The application communicates with a locally running Express.js API to fetch and display user profile data.

The app displays a paginated list of profiles and allows navigation to a detailed profile screen where additional information is fetched dynamically from the API.

This project focuses on real-world mobile development concepts such as API integration, asynchronous operations, pagination, navigation, environment variables, and robust error handling.

---

## Technologies Used
- React Native (Expo)
- Axios
- Express.js (Local API Server)
- React Navigation (Native Stack)
- JavaScript (ES6+)

---

## Features
- Fetch profiles from a REST API
- Paginated profile list using FlatList
- Dynamic profile detail screen
- Stack navigation between list and detail screens
- Environment variable based API configuration
- Pull-to-refresh functionality
- Global API error handling using Axios interceptors
- Loading, empty, and error states for better user experience

---

## API Configuration
The application connects to a locally running Express.js server.  
The API base URL is configured using Expo environment variables to allow access from a physical mobile device.

Example `.env` file:
```env
EXPO_PUBLIC_API_BASE_URL=http://192.168.1.6:3000


# Application Structure
ProfilesApp/
├── api/
│   └── client.js
├── screens/
│   ├── ProfilesListScreen.js
│   └── ProfileDetailScreen.js
├── assets/
├── App.js
├── app.json
├── package.json
└── README.md

Start the API Server
cd ProfilesServer
npm install
node server.js
cd ProfilesApp
npm install
npx expo start
