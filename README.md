# FastAPI Notes App 📝

A simple FastAPI application for managing notes, using MongoDB for data storage and Jinja2 for rendering templates.

---

## 🚀 Features
- ✅ Create, Read, Update, and Delete (CRUD) notes
- ✅ Mark notes as important
- ✅ Uses FastAPI with Jinja2 templates for frontend rendering
- ✅ MongoDB integration for data persistence
- ✅ API documentation with Swagger UI

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/Danish1042/fastapi_tut.git
cd fastapi_tut
```

### 2️⃣ Create & Activate a Virtual Environment
#### Windows (PowerShell):
```sh
python -m venv venv
venv\Scripts\activate
```
#### macOS/Linux:
```sh
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

### 4️⃣ Start MongoDB
Ensure MongoDB is running locally or provide a connection string in `config/db.py`.

### 5️⃣ Run the FastAPI Server
```sh
uvicorn index:app --reload
```

### 6️⃣ Open in Browser
- **Swagger UI (API Docs):** [`http://127.0.0.1:8000/docs`](http://127.0.0.1:8000/docs)
- **Redoc (Alternative Docs):** [`http://127.0.0.1:8000/redoc`](http://127.0.0.1:8000/redoc)

---

## 📂 Project Structure
```
fastapi_tut/
│── routes/           # API routes
│── templates/        # HTML templates (Jinja2)
│── config/           # Database configuration
│── static/           # CSS/JS files
│── index.py          # Main FastAPI app
│── .gitignore        # Ignore unnecessary files
│── README.md         # Project documentation
│── requirements.txt  # Project dependencies
```

---

## 📌 API Endpoints
| Method | Endpoint  | Description |
|--------|----------|-------------|
| POST   | `/note/` | Create a new note |
| GET    | `/notes/` | Fetch all notes |
| GET    | `/note/{id}` | Fetch a specific note |
| PUT    | `/note/{id}` | Update a note |
| DELETE | `/note/{id}` | Delete a note |

---

## 📝 How to Ignore Virtual Environment (Git)
If you don't want to push the `venv` folder to GitHub, add the following line to your `.gitignore` file:
```
venv/
```

---

## 📌 Contributing
Feel free to fork the repository and submit pull requests. Contributions are welcome! 🚀

---

## 📝 License  
This project is open-source. Feel free to use and modify it! 😊

