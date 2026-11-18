# 🌱 CropMart

### Connecting Farmers, Buyers, and Smarter Agriculture

CropMart is a full-stack agricultural marketplace designed to connect farmers and buyers through a unified digital platform. It brings together agricultural product listings, market price insights, demand forecasting, smart matching, and route optimization.

The goal is to make agricultural trading more accessible, informed, and efficient.

---

## ✨ Features

- **User Authentication:** Registration and login with secure password hashing and JWT-based authentication.
- **Agricultural Marketplace:** Browse and manage agricultural product listings.
- **Market Price Insights:** Access market price information to support better buying and selling decisions.
- **Demand Forecasting:** Prototype forecasting functionality to estimate product demand.
- **Smart Matching:** Match relevant agricultural requirements with available products.
- **Route Optimization:** Generate optimized routes for agricultural delivery planning.
- **REST API:** Backend API built with FastAPI.
- **Interactive Interface:** Browser-based frontend built using HTML, CSS, and JavaScript.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python, FastAPI |
| Database | SQLite |
| ORM | SQLAlchemy |
| Authentication | JWT |
| Password Hashing | Passlib, bcrypt |
| API Testing / Documentation | FastAPI Swagger UI |

---

## 📁 Project Structure

```text
CropMart/
│
├── backend/
│   ├── app/
│   │   ├── core/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── services/
│   │   ├── routers/
│   │   └── main.py
│   │
│   ├── requirements.txt
│   └── app/ 
│
├── index.html
├── style.css
├── script.js
├── logo.png
├── logo-128.png
├── .gitignore
└── README.md
```

---

## ⚙️ Getting Started

Follow these steps to run CropMart locally.

### 1. Clone the repository

```bash
git clone https://github.com/IMyash5/CropMart.git
cd CropMart
```

### 2. Create a Python virtual environment

Python 3.12 is recommended.

```bash
py -3.12 -m venv backend/.venv
```

### 3. Install dependencies

On Windows:

```powershell
.\backend\.venv\Scripts\python.exe -m pip install -r backend/requirements.txt
```

### 4. Navigate to the backend directory

```powershell
cd backend
```

### 5. Initialize demo data (optional)

For a fresh local database, run:

```powershell
.\.venv\Scripts\python.exe -m app.seed
```

**Note:** Run the seed command only when setting up a fresh database. Back up any existing database before initializing demo data.

### 6. Start the application

```powershell
.\.venv\Scripts\python.exe -m uvicorn app.main:app --reload
```

### 7. Open CropMart

Visit:

- **Application:** http://127.0.0.1:8000
- **API Documentation:** http://127.0.0.1:8000/docs
- **Health Check:** http://127.0.0.1:8000/health

---

## 🔌 API

CropMart provides REST API endpoints for its application modules.

The API is organized around:

- Authentication
- Products
- Orders
- AI-powered features
- Agricultural requirements

Explore the interactive Swagger documentation at `/docs` after starting the backend.

---

## 🔐 Security Notes

- Passwords are hashed before storage.
- JWT tokens are used for authentication.
- Local database files and environment secrets should not be committed to GitHub.
- The current project is a development prototype. Review configuration, secret management, CORS, and authorization before production deployment.

---

## 🚀 Future Improvements

- Integration with real-time agricultural market data.
- More advanced demand forecasting models.
- Secure online payment gateway integration.
- Improved inventory and order management.
- Deployment with cloud database support.
- Automated backend testing.
- Enhanced analytics dashboards for farmers and buyers.

---

## 👨‍💻 Project Status

**Status:** Active Development

CropMart is an evolving project. Features and architecture may be improved as development progresses.

---

## 📄 License

No license has been added yet. All rights are reserved by the repository owner unless a license is added.