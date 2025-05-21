# 🤖 AI Integration with FastAPI

This project is a backend service built using **FastAPI** to integrate AI-powered features. It includes CORS support for frontend communication and uses modular route-based architecture for maintainability.

---

## 🚀 Features

- ⚡ FastAPI backend for AI services  
- 🔄 CORS enabled for frontend/backend communication  
- 🔌 Modular route handling (e.g., `send_msg`)  
- 🌐 Port configuration via environment variables  
- 🚀 Ready for local development and deployment  

---

## 📁 Project Structure
- ai-integration/
- main.py .. Entry point of the FastAPI app
- route/
- │ └── send_msg.py # Handles AI-related requests
- ├── requirements.txt # Python dependencies
- └── README.md # Project documentation

---

## 🧪 Getting Started

### 1. Clone the Repository


git clone https://github.com/BaburSadiqi/Fast-AI-Chat.git
cd Fast-AI-Chat

### 2. Create and Activate a Virtual Environment (Optional)
- python -m venv venv
- source venv/bin/activate  # On Windows: venv\Scripts\activate

### 3. Install Dependencies
- pip install fastapi uvicorn


---

# 🚀 Run the Application
- uvicorn main:app --reload
- App will be running at: http://127.0.0.1:8000

---

# 🔌 API Endpoint
| Method | Endpoint    | Description              |
| ------ | ----------- | ------------------------ |
| POST   | `/send-msg` | Handles AI chat messages |

(Assumes your send_msg.py defines the /send-msg route)

# ⚙️ Environment Variables
| Variable | Description            | Default |
| -------- | ---------------------- | ------- |
| `PORT`   | Port to run the server | `8000`  |

## To run with a specific port:
- PORT=5000 uvicorn main:app
---

## 📦 Deployment
- uvicorn main:app --host 0.0.0.0 --port ${PORT}

---
# 👤 Author
Babur Sadiqi
