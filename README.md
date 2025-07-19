# KPA Backend Assignment - FastAPI

## 📌 Assignment Overview
This project is developed as part of the KPA assignment to demonstrate backend development skills using **FastAPI** and **PostgreSQL**. Two functional APIs were implemented based on the provided Postman collection.

---

## 🚀 Tech Stack

- **Backend:** Python (FastAPI)
- **Database:** PostgreSQL
- **Testing:** Postman
- **ORM:** SQLAlchemy
- **Others:** Pydantic, Uvicorn

---

## 🧩 Implemented APIs

### ✅ 1. User Registration API (POST `/users/`)
- Registers a new user with hashed password.
- Stores data in PostgreSQL.
- Validates unique email.

### ✅ 2. File Upload API (POST `/upload/`)
- Accepts and stores a file (PDF, image, etc.)
- Returns file details on success.

---

## 🔗 Resources Used
- 📁 Postman Collection: `KPA_form data.postman_collection.json`
- 🌐 SwaggerHub Docs: [Link](https://app.swaggerhub.com/apis/sarvasuvidhaen/kpa-form_data/1.0.0)
- 💻 Frontend Repo: [KPA-ERP-FE](https://github.com/s2pl/KPA-ERP-FE/)
- 🧪 Hosted API Reference: [kpa.suvidhaen.com](https://kpa.suvidhaen.com)

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/kpa-fastapi-backend.git
   cd kpa-fastapi-backend


   Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Start PostgreSQL and update credentials in database.py.

Run the app

bash
Copy
Edit
uvicorn main:app --reload
Test APIs using Postman with the updated collection.

📩 Postman Collection
Updated Postman collection with working APIs is available in the repo.

