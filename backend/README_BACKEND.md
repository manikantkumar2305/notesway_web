# NotesWay Backend

## Overview
This is the **backend service** for **NotesWay**, built using **Python** with a clean and modular architecture.
It provides RESTful APIs for authentication, user management, file handling, and academic note operations.

The backend is designed to be **secure, scalable, and production-ready**, and integrates with a React-based frontend.

---

## Tech Stack
- Python
- FastAPI
- MongoDB (MongoDB Atlas)
- Motor (Async MongoDB Driver)
- JWT Authentication
- Uvicorn (ASGI Server)

---

## Project Structure
```
backend/
├── core/          # Application configuration
├── middleware/    # Custom middleware
├── models/        # Database models
├── routers/       # API routes
├── schemas/       # Pydantic schemas
├── services/      # Business logic
├── utils/         # Utility functions
├── main.py        # Application entry point
├── database.py    # Database connection logic
├── requirements.txt
└── .env.example
```

---

## Getting Started

### Prerequisites
- Python 3.10 or higher
- Virtual environment (recommended)
- MongoDB (local or Atlas)

---

### Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate    # Linux / macOS
venv\Scripts\activate     # Windows
```

---

### Install Dependencies
```bash
pip install -r requirements.txt
```

---

### Environment Variables
Create a `.env` file inside the `backend/` directory using `.env.example`:

```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET_KEY=your_secret_key
```

⚠️ Do not commit `.env` files to version control.

---

### Run Development Server
```bash
uvicorn main:app --reload
```

Server will be available at:
```
http://localhost:8000
```

---

## API Documentation
FastAPI automatically generates API docs:

- Swagger UI:
  http://localhost:8000/docs

- ReDoc:
  http://localhost:8000/redoc

---

## Security
- JWT-based authentication
- Environment-based configuration
- Secure database connectivity
- Role-based access control

---

## Notes
- Communicates with a **React frontend**
- Designed for cloud deployment
- Follows clean architecture principles

---

## Author
Manikant Kumar

---

## License
This project is intended for educational, portfolio, and demonstration purposes.
