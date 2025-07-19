#  KPA Backend Assignment

## Author
**Nishmitha**

##  Tech Stack
- **Backend Framework**: FastAPI
- **Database**: PostgreSQL
- **ORM**: SQLAlchemy
- **Schema Validation**: Pydantic
- **Server**: Uvicorn
- **API Testing**: Postman

---

## Features Implemented

### 1. **User Registration API**
- **Route**: `/users`
- **Method**: `POST`
- **Description**: Register a new user with name, email, and password.
- **Security**: Passwords are hashed using `passlib` before storing in the database.
- **Validation**: Duplicate email check included.

### 2. **File Upload API**
- **Route**: `/uploadfile/`
- **Method**: `POST`
- **Description**: Uploads a file (any format). Stores it in a local `uploads/` directory.
- **Validation**: Checks for presence of file.

---

## 📦 Setup Instructions

### 1. Clone the repository
```bash
git clone <your_repo_url>
cd kpa_assignment

Create a virtual environment & activate
bash
Copy
Edit
python -m venv venv
# Windows:
venv\Scripts\activate
# Linux/macOS:
source venv/bin/activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Set up PostgreSQL Database
Create a new database (e.g., kpa_db)

Update database.py with your PostgreSQL username, password, and DB name.

Example:

python
Copy
Edit
SQLALCHEMY_DATABASE_URL = "postgresql://username:password@localhost/kpa_db"
5. Run the FastAPI Server
bash
Copy
Edit
uvicorn main:app --reload
6. Open API Docs
Visit http://127.0.0.1:8000/docs to test APIs via Swagger UI.

📬 Postman Collection
Exported Postman collection:
KPA_form data.postman_collection.json
✅ Includes working examples of User Registration and File Upload.

📝 Screenshots (Optional)
(Insert screenshots of Swagger UI, Postman results, database output if needed)


⚙️ Project Structure
pgsql
opy
Edit
.
├── main.py
├── models.py
├── schemas.py
├── database.py
├── routes/
│   ├── user.py
│   └── upload.py
├── uploads/
├── requirements.txt
├── README.md
└── KPA_form data.postman_collection.json
⚠️ Known Limitations
Files are stored locally; could be extended to AWS S3 or cloud.

Basic validation added; further checks (like file size/type limits) can be implemented.

💡 Future Improvements
Environment variables using .env

Dockerization of the app

Add JWT authentication

Form submission API integration

📧 Contact
Have questions? Email me at: nishmthanishu77@gmail.com
yaml
Copy
Edit

---

Let me know if you'd like a version with screenshots or help writing `.env` or `requirements.txt