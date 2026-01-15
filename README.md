🤖AI Chat Application (Django)

A Django-based AI chat application that supports intelligent conversations, document uploads, document summarization, and document-based question answering.  
The project follows clean architecture principles with strong focus on code quality, maintainability, and scalability.

---

🌟 Features

- Secure user authentication (Signup & Login)
- AI-powered conversational interface
- Upload and process documents
- Automatic text extraction from files
- Document summarization using AI
- Ask questions directly from uploaded documents
- Chat history management per user
- Django Admin panel integration
- High code quality with Pylint validation

---

🛠️ Technology Stack

| Layer | Technology |
|------|-----------|
| Backend | Django 6.0.1 |
| Frontend | HTML, CSS, JavaScript |
| Database | SQLite |
| AI Service | Groq API |
| Document Processing | PyMuPDF, pdfplumber, python-docx, openpyxl |
| Code Quality | Pylint |

---

📂 Project Structure

chatapp/
├── chat/                      # Core application logic
│   ├── admin.py               # Admin panel configuration
│   ├── apps.py                # App configuration
│   ├── models.py              # Database models
│   ├── urls.py                # App-level URL routing
│   ├── views.py               # Request handling & business logic
│   └── document_processor.py  # Document text extraction utilities
│
├── templates/                 # HTML templates
│   ├── index.html             # Main chat interface
│   ├── login.html             # User login page
│   └── signup.html            # User registration page
│
├── chatapp/                   # Project configuration
│   ├── settings.py            # Django settings
│   ├── urls.py                # Project-level URL routing
│   ├── asgi.py                # ASGI configuration
│   └── wsgi.py                # WSGI configuration
│
├── manage.py                  # Django management commands
├── requirements.txt           # Project dependencies
├── .pylintrc                  # Pylint configuration
└── .gitignore                 # Git ignore rules


⚙️ Setup Instructions

1. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate

2. Install Dependencies
bash
pip install -r requirements.txt

3. Environment Configuration
Create a .env file in the root directory:env
SECRET_KEY=your_django_secret_key
GROQ_API_KEY=your_groq_api_key
GROQ_MODEL=llama-3.1-8b-instant

4. Database Setup
bash
python manage.py migrate

5. Create Superuser
bash
python manage.py createsuperuser

6. Run the Application
bash
python manage.py runserver

🔍 Code Quality & Standards
Static code analysis using Pylint

Django-compatible linting configuration

Modular and readable codebase

Pylint Score: 9.67 / 10

🧑‍💻Run code quality check:
bash
$env:DJANGO_SETTINGS_MODULE="chatapp.settings"
pylint chat/chatapp

📌 Design Highlights
Clean MVC architecture

Session-based conversation handling

Modular document processing pipeline

Secure authentication flow

Scalable backend structure

👩‍💻 Author
Princy Angeline J

📄 License
This project is intended for educational, Internship and demonstration purposes.
