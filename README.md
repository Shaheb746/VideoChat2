# 🎥 VideoCat

> A Modern Real-Time Video Conferencing Platform built using WebRTC, React, Node.js, and Socket.IO.

![Landing](https://raw.githubusercontent.com/Shaheb746/VideoChat/main/Frontend/public/landing.png)

![Meeting](https://raw.githubusercontent.com/Shaheb746/VideoChat/main/Frontend/public/meeting.png)

![Dashboard](https://raw.githubusercontent.com/Shaheb746/VideoChat/main/Frontend/public/dashboard.png)

---

# 🚀 Features

✅ Real-Time Video Calling  
✅ Multi-User Meeting Rooms  
✅ Peer-to-Peer Communication  
✅ Live Chat System  
✅ Screen Sharing  
✅ Camera ON/OFF  
✅ Microphone Mute/Unmute  
✅ Responsive UI  
✅ WebRTC Signaling  
✅ Room-Based Communication  
✅ Dynamic Video Rendering  
✅ Meeting Join & Leave Notifications  
✅ Fast Low-Latency Communication  
✅ Browser-Based Video Meetings  
✅ Simple & Clean User Interface  
✅ Dynamic Participant Handling  
✅ Real-Time Socket Communication  

---

# 🧠 About The Project

VideoCat is a modern browser-based video conferencing platform that allows users to communicate in real-time using audio, video, and chat features.

The application uses WebRTC for peer-to-peer media communication and Socket.IO for signaling between connected users.

This project is designed for developers who want to learn:
- WebRTC Fundamentals
- Socket.IO Signaling
- Real-Time Communication
- Peer-to-Peer Networking
- Video Streaming
- Media Stream Handling
- Frontend & Backend Integration
- Real-Time Event Systems

---



# 🏗️ Architecture

## Current Architecture → Mesh (P2P)

In Mesh Architecture, every participant directly connects with every other participant.

### Example

- 2 Users → 1 Connection
- 3 Users → 3 Connections
- 4 Users → 6 Connections
- 5 Users → 10 Connections

### Architecture Flow

```text
User A  ←→  User B
   ↕           ↕
User C  ←→  User D

```
# Complete Application Flow


```
React Frontend
       │
       │ Socket.IO Signaling
       ▼
Node.js Signaling Server
       │
       ▼
WebRTC Peer Connections
       │
       ▼
Real-Time Audio/Video Streams

```



# ⚡ Technology Stack

## Frontend Technologies
- React.js
- React Router DOM
- Bootstrap
- CSS3
- Socket.IO Client
- WebRTC APIs

## Backend Technologies
- Node.js
- Express.js
- Socket.IO
- CORS

## Real-Time Communication Technologies
- WebRTC
- RTCPeerConnection
- RTCIceCandidate
- SDP (Session Description Protocol)
- STUN Server



# 🔄 WebRTC Working Flow

## Step 1 → User Opens Application

- Browser loads frontend
- Camera permission requested
- Microphone permission requested

## Step 2 → User Joins Room
- User enters meeting room
- Socket.IO establishes connection

## Step 3 → Signaling Process Starts

Socket.IO exchanges:
- Offer
- Answer
- ICE Candidates
  
## Step 4 → Peer Connection Established

``` RTCPeerConnection ```creates direct communication between peers.

## Step 5 → Media Streams Shared
- Audio stream shared
- Video stream shared
- Remote streams rendered dynamically


# 📂 Folder Structure
```
  VideoCat/
│
├── Backend/
│   ├── app/
│   │   ├── controllers/
│   │   ├── dbinit/
│   │   ├── middleware/
│   │   ├── models/
│   │   └── routes/
│   ├── index.js
|   ├── package-lock.json
│   └── package.json
│
├── Frontend/
│   ├── public/
│   ├── src/
│   ├── eslint.config.js
|   ├── environment.js
|   ├── index.html
|   ├── package-lock.json
|   ├── package.json
│   ├── README.md
|   ├──.gitignore
│   └── vite.config.js
│
├── README.md
└── .gitignore
```

# 🔌 Socket.IO Events
### Client → Server
```
join-call
signal
chat-message
screen-share
disconnect
```

### Server → Client
```
user-joined
user-left
signal
chat-message
```

# 🎥 WebRTC APIs Used
### getUserMedia()

Used to access:

- Camera
- Microphone
```
navigator.mediaDevices.getUserMedia({
  video: true,
  audio: true
});
```

# RTCPeerConnection()

Used to establish peer-to-peer connection.
```
new RTCPeerConnection(configuration);
```

# addTrack()

Used to add media tracks into peer connection.
```
stream.getTracks().forEach(track => {
  peerConnection.addTrack(track, stream);
});
```

# 🌍 STUN Server Configuration
```
const peerConnectionConfig = {
  iceServers: [
    {
      urls: "stun:stun.l.google.com:19302"
    }
  ]
};

```

# 🛡️ Security Features

✅ Encrypted WebRTC Communication
✅ Browser Permission Control
✅ Room-Based Isolation
✅ Secure Socket Signaling
✅ Peer-to-Peer Media Transfer

# 📱 Responsive Design

VideoCat supports:

- Desktop Devices
- Tablets
- Mobile Phones

# 🚀 Installation Guide
Clone Repository
```
git clone https://github.com/yourusername/videocat.git
```

# Install Frontend Dependencies
```
cd client
npm install
```

# Install Backend Dependencies
```
cd server
npm install
```

# ▶️ Run Application
Run Frontend
```
npm run dev
```

# 🌐 Browser Support
```
| Browser | Support |
| ------- | ------- |
| Chrome  | ✅       |
| Edge    | ✅       |
| Firefox | ✅       |
| Brave   | ✅       |

```

# 📈 Future Improvements

🚀 Authentication System
🚀 Meeting Recording
🚀 File Sharing
🚀 AI Noise Cancellation
🚀 Live Captions
🚀 Admin Controls
🚀 Cloud Deployment
🚀 SFU Architecture
🚀 Meeting Scheduling

# 🔗 Useful Resources
- https://webrtc.org/
- https://socket.io/
- https://react.dev/
- https://nodejs.org/
- https://developer.mozilla.org/en-US/docs/Web/API/WebRTC_API

