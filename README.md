# EchoSphere Frontend

## Overview
EchoSphere Frontend is the **official frontend** for [EchoSphere](https://github.com/Isomorphismss/echo-sphere), a distributed real-time messaging platform. Built with **Uni-APP + Vue**, it supports **mini-program, H5, and mobile app clients**.  

### **Features**
- **User Authentication**: Phone number login/registration with **SMS verification**.
- **Real-Time Messaging**: One-on-one and group chat with **Netty WebSocket auto-reconnection**.
- **Social Feeds**: Post, like, and comment on **moments**.
- **Multi-Device Support**: Log in from **multiple devices** simultaneously with synchronized data.
- **Caching & Performance**: Local **image and chat history caching** for faster load times.
- **Personalization**: Customizable **profile settings and friend lists**.

## **Tech Stack**
- **Frontend**: Uni-APP, Vue
- **State Management**: Vuex
- **Networking**: WebSocket (**Netty**), HTTP (**Axios**)
- **Caching**: LocalStorage, Image Caching
- **UI Components**: Vant, Uni-UI

## **Getting Started**
### **1️⃣ Prerequisites**
Before running the frontend, make sure the **backend services** and **Netty server** from [EchoSphere Backend](https://github.com/Isomorphismss/echo-sphere) are running.

### **2️⃣ Installation**
Clone the repository:
```sh
git clone https://github.com/Isomorphismss/echo-sphere-frontend.git
cd echo-sphere-frontend
```
Install dependencies:
```sh
npm install
```
### **3️⃣ Configuration**
Update the backend API and Netty server URLs in `App.vue`:
```javascript
const backendUrl = 'http://your-backend-ip:port';
const nettyUrl = 'ws://your-netty-ip:port';
```
⚠️ For Android emulator testing, replace localhost with your local network IP.

### **4️⃣ Running the Project**
Start the development server:
```sh
npm run dev
```
Access the frontend on different platforms:
- **H5**: Open in a browser
- **Mini-Program**: Compile and run via Uni-APP IDE.
- **Mobile App**: Run on an Android emulator or a physical device.

## **Usage**
- Login/Register: Use your phone number to register/log in (SMS verification required).
- Chat: Start one-on-one/group chats. The app will auto-reconnect if the connection is lost.
- Moments: Post updates, like, and comment on friends' moments.
- Profile: Customize your personal profile and manage your friend list.
- Multi-Device Login: Log in from multiple devices simultaneously.

## **Caching & Performance**
- Chat History: Messages are cached locally for quick access.
- Image Caching: Cached images reduce load times and improve performance.
- Auto-Reconnection: The app reconnects automatically if disconnected from the Netty server.

## **Notes**
- Ensure the backend services and Netty server are running before starting the frontend.
- For Android emulator testing, update the IP address in `App.vue` to your local network IP.
- Multi-device login allows users to access their accounts from multiple devices simultaneously.

## **License**
This project is licensed under the **MIT License**.
