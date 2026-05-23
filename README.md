# VideoCat 🎥
## Real-Time Video Meeting & Collaboration Platform

VideoCat is a modern real-time video conferencing application built using WebRTC, React, Node.js, and Socket.IO.


### It allows users to create or join meeting rooms instantly with features like:

- 🎥 Real-time video/audio calling 
- 🖥️ Screen sharing
- 💬 Live chat
- 🔐 Secure peer-to-peer communication
- 👥 Multi-user meeting rooms
- ⚡ Low latency communication
- 📱 Responsive UI
- 🌐 Browser-based communication



# 🧠 About The Project

VideoCat is a real-time communication platform that allows users to create and join video meetings directly in the browser.

This project is built mainly for:
- Learning WebRTC
- Understanding Socket.IO signaling
- Real-time communication systems
- Peer-to-peer networking
- Video conferencing architecture


# 🏗️ Architecture

Every participant directly connects with every other participant.


# ⚡ Tech Stack
### Frontend
- React.js
- React Router DOM
- Bootstrap / CSS
- Socket.IO Client
- WebRTC APIs
  
### Backend
- Node.js
- Express.js
- Socket.IO
- CORS
  
### Real-Time Technologies
- WebRTC
- STUN Server
- RTCPeerConnection
- RTCIceCandidate
- SDP Negotiation

# 📂 Folder Structure  


# 🔄 WebRTC Working Flow
### 1. User Opens Application
- Camera permission requested
- Microphone permission requested
### 2. User Joins Room
- Socket connection established
- User joins meeting room
### 3. Signaling Process Starts
- Socket.IO exchanges:
- Offer
- Answer
- ICE Candidates
### 4. Peer Connection Established
- RTCPeerConnection connects users directly.
### 5. Media Streams Shared
- Audio stream shared
- Video stream shared

# 🔌 Socket.IO Events
### Client → Server
```
join-call
signal
chat-message
disconnect
```
# Server → Client
```
user-joined
user-left
signal
chat-message
```

# 🎥 WebRTC APIs Used
### getUserMedia()


