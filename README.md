# EchoSphere Frontend  

## 🌟 Introduction  
EchoSphere Frontend is the official frontend for **EchoSphere**, a distributed, real-time messaging platform.  
It is built with **Uni-APP + Vue**, supporting **H5, mini-programs, and mobile apps**.

🔗 **Backend Repository:** [EchoSphere Backend](https://github.com/Isomorphismss/echo-sphere)  
⚠️ **Make sure the backend is running before starting the frontend.**  

## 🚀 Getting Started  

### 1️⃣ Prerequisites  
- Follow the instruction in the backend README, ensure the **backend services** and **Netty server** are running.  
- Install **Node.js (16+)** and **npm**.  

### 2️⃣ Installation  
```sh
git clone https://github.com/Isomorphismss/echo-sphere-uniapp.git
cd echo-sphere-uniapp
npm install
```

### 3️⃣ Configuration  
Modify `App.vue` to set the **backend API** and **WebSocket server** URLs:  
```javascript
const backendUrl = 'http://your-backend-ip:port';
const nettyUrl = 'ws://your-netty-ip:port';
```
⚠️ **For Android emulator testing**, replace `localhost` with your local network IP.

### 4️⃣ Running the Project  
Start the development server:  
```sh
npm run dev
```
Available platforms:  
- **H5**: Open in a browser.  
- **Mini-Program**: Compile in Uni-APP IDE.  
- **Mobile App**: Run on an emulator or a physical device.  

## 📝 Notes  
- **Backend dependency**: The frontend requires the backend to be running for full functionality.  
- **Multi-device login**: Users can log in from multiple devices simultaneously.  
- **Offline mode**: Messages are cached locally for faster access.  


## 📜 License  
This project is licensed under the **MIT License**.  
