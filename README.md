# SyncChat--Backend  
**Real-time AI-powered chat application with Google Gemini AI**  

## 📝 About  
Sync Chat is a **real-time, AI-powered chat application** designed for **team collaboration, project-based discussions, and AI-assisted code generation**. It integrates **Google Gemini AI** to provide intelligent coding suggestions and structured file creation, making it a powerful tool for developers and teams.  

## 🚀 Features  
- **Real-time messaging** with **Socket.IO** for seamless team communication.  
- **AI-powered code generation** using **Google Gemini AI (gemini-1.5-flash)**.  
- **Project-based group discussions** with structured file management.  
- **Optimized MongoDB schema** for storing project-based conversations and AI-generated files.  
- **Redis caching** for performance improvements and real-time data sync.  
- **JWT authentication** for secure user access.  

---

## 🛠 Tech Stack  
| Technology | Purpose |  
|------------|---------|  
| **Node.js & Express.js** | Backend framework & API handling |  
| **MongoDB** | Database for structured project discussions & AI-generated files |  
| **Socket.IO** | Real-time messaging |  
| **Redis** | Caching & real-time data sync |  
| **Google Gemini API** | AI-powered code generation |  
| **JWT (JSON Web Token)** | Secure authentication |  

---

## ⚙️ Installation & Setup  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/adityaprajapati10/SyncChat--Backend.git
cd SyncChat--Backend
```

### 2️⃣ Install Dependencies
```sh
npm install
```
### 3️⃣ Configure Environment Variables
#### Create a .env file in the root directory and add the following:
```sh
PORT=your_port
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
REDIS_HOST=your_redis_host
REDIS_PORT=your_redis_port
REDIS_PASSWORD=your_redis_password
GOOGLE_AI_KEY=your_google_gemini_api_key
```
### 4️⃣ Start the Server
```sh
npm start
```

### The backend should now be running on http://localhost:PORT 🚀

## 📌 API Endpoints  

| Method | Endpoint          | Description |
|--------|------------------|-------------|
| **GET**  | `/`               | Check server status |
| **POST** | `/users/login`     | User authentication |
| **POST** | `/users/register`  | User registration |
| **GET**  | `/projects`        | Fetch user projects |
| **POST** | `/projects`        | Create a new project |
| **POST** | `/ai/generate`     | AI-powered code generation using Google Gemini API |

📢 **More endpoints are available in the respective route files (`userRoutes.js`, `projectRoutes.js`, `aiRoutes.js`).**  
