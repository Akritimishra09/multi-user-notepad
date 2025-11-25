# Cloud Notepad Conference

## Overview
Cloud Notepad Conference is a collaborative note-taking web application that integrates real-time chat functionality and an AI chatbot feature. This application allows users to create, edit, and manage notes while engaging in discussions through a chatroom that functions as a digital conference room.

## Features
- **Collaborative Note-taking**: Users can create and edit notes in real-time.
- **Chatroom**: A dedicated chatroom for users to communicate and collaborate effectively.
- **AI Chatbot**: An AI-powered chatbot that assists users by providing suggestions, summarizing notes, and answering queries.
- **User Presence**: Displays online status of users in the chatroom.

## Technologies Used
- **Frontend**: React, TypeScript, CSS
- **Backend**: Node.js, Express, TypeScript
- **Database**: MongoDB (or any other preferred database)
- **Real-time Communication**: Socket.io
- **AI Integration**: Custom AI service for chatbot functionality

## Project Structure
```
cloud-notepad-conference
├── backend
│   ├── src
│   │   ├── index.ts
│   │   ├── server.ts
│   │   ├── config
│   │   │   └── index.ts
│   │   ├── routes
│   │   │   ├── notes.ts
│   │   │   └── chat.ts
│   │   ├── controllers
│   │   │   ├── notesController.ts
│   │   │   └── chatController.ts
│   │   ├── services
│   │   │   ├── realtime.ts
│   │   │   └── ai.ts
│   │   ├── models
│   │   │   ├── note.ts
│   │   │   └── message.ts
│   │   └── types
│   │       └── index.d.ts
│   ├── package.json
│   └── tsconfig.json
├── frontend
│   ├── public
│   │   └── index.html
│   ├── src
│   │   ├── main.tsx
│   │   ├── App.tsx
│   │   ├── api
│   │   │   └── client.ts
│   │   ├── components
│   │   │   ├── Editor/
│   │   │   │   ├── Editor.tsx
│   │   │   │   └── Editor.css
│   │   │   ├── Sidebar/
│   │   │   │   ├── Sidebar.tsx
│   │   │   │   └── Sidebar.css
│   │   │   ├── ChatRoom/
│   │   │   │   ├── ChatRoom.tsx
│   │   │   │   └── ChatRoom.css
│   │   │   ├── AIChat/
│   │   │   │   ├── AIChat.tsx
│   │   │   │   └── AIChat.css
│   │   │   └── Presence/
│   │   │       ├── PresenceBar.tsx
│   │   │       └── Presence.css
│   │   ├── hooks
│   │   │   ├── useRealtime.ts
│   │   │   └── useAutosave.ts
│   │   ├── stores
│   │   │   └── notesStore.ts
│   │   ├── styles
│   │   │   └── theme.css
│   │   └── types
│   │       └── index.d.ts
│   ├── package.json
│   └── tsconfig.json
├── docker-compose.yml
├── .env.example
├── .gitignore
└── README.md
```

## Setup Instructions
1. **Clone the Repository**:
   ```
   git clone <repository-url>
   cd cloud-notepad-conference
   ```

2. **Backend Setup**:
   - Navigate to the backend directory:
     ```
     cd backend
     ```
   - Install dependencies:
     ```
     npm install
     ```
   - Start the backend server:
     ```
     npm run start
     ```

3. **Frontend Setup**:
   - Navigate to the frontend directory:
     ```
     cd ../frontend
     ```
   - Install dependencies:
     ```
     npm install
     ```
   - Start the frontend application:
     ```
     npm run start
     ```

4. **Access the Application**:
   Open your browser and navigate to `http://localhost:3000` to access the Cloud Notepad Conference application.

## Contribution
Contributions are welcome! Please feel free to submit a pull request or open an issue for any enhancements or bug fixes.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.