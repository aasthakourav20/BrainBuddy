# BrainBuddy
## A mental health chat assistant

BrainBuddy is a mental health **AI** powered chat assistant that guides and helps you to improve your mental health.
BrainBuddy website provides a user-friendly UI to learn about mental health.

## Features

- AI chat assistant to take guidance about mental health.
- Analyse your mental health over a period of time.
- Get an Indication about your mental health condition with a graphical visualization.
- Editor's compiled articles to read and educate about mental health problems.
- Get emails from time to time with suggestions to improve your mental health.



## Tech

#### System Design
BrainBuddy application runs on 4 server
- Frontend
- Backend
- WebSocket Server
- Email Server


#### Tech stack
- Frontend
  - React JS
  - Tailwind
- Backend
  - Node Js
  - Express Js
  - Gemini (Gen AI)
  - Web Sockets
  - Node Mailer
- Tools
  - Vercel
  - Render
  - Mongo DB
  - Firebase
 
## How to Setup Locally?
### Firebase Setup
  1. Setup a new Firebase project
  2. Add a Web App
  3. Go to Authentication -> Sign-in Method
  4. Enable Email/Password, Gmail as Provider
  5. Go to the Project Settings of Web App and get your ```firebaseConfig``` object
  6. Create ```.env``` in Frontend folder and add ```firebaseConfig``` as per ```.env.sample``` file
  7. In the service accounts section, Generate ```new private key``` (json object).
  6. Create ```.env``` in Backend folder and add ```new private key``` as per ```.env.sample``` file
  8. Fill rest ```.env``` as per ```.env.sample``` files
### Gemini Setup
  - Get your Gemini (by Google) ```API_KEY``` from (https://ai.google.dev) and put in Backend ```.env``` as per ```.env.sample```
### MongoDB Setup
  - Create a MongoDB Atlas (https://www.mongodb.com) account and get your ```URI``` and put in Backend ```.env``` as per ```.env.sample```
### Create Connection amongst Servers
  - Put Url for Websocketserver in Backend .env (ex- ```WEBSOCKET_SERVER=ws://localhost:8802```)
  - Put Url for Backend and Websocketserver in Frontend .env (ex- ```REACT_APP_API_LINK=http://localhost:8800``` and ```REACT_APP_WS_LINK=ws://localhost:8802```)
### Scripts to Install and Run
  1. Need to have ```Node.js``` installed
  2. Go to the Backend, Frontend, Websockerserver folder seperately and run for each ```npm install```
  3. Run Backend by, ```npm run dev``` or ```npm start```
  4. Run Frontend by, ```npm start```
  5. Run Websocketserver by, ```node index.js```
  
    
## Website Preview

#### HomePage 
![Screenshot (296)](https://github.com/aasthakourav20/BrainBuddy/assets/148269962/86672a12-eff7-47e0-a2cf-91af9f83c625)

#### Analysis
![Screenshot (300)](https://github.com/aasthakourav20/BrainBuddy/assets/148269962/2f63e6ea-3bf7-4976-a104-c1cc470e4372)

#### AI Chat
![Screenshot (299)](https://github.com/aasthakourav20/BrainBuddy/assets/148269962/60254632-1a2e-4842-b933-e3214b3db629)



