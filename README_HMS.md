
# 🏥 Hospital Management System (HMS)

## 📌 Project Overview

The **Hospital Management System (HMS)** is a web-based application developed using **Django** and **MySQL**, aimed at automating hospital operations such as patient registration, doctor management, appointment scheduling, and billing. The system provides separate interfaces for administrators, doctors, and patients to enhance hospital workflow efficiency and reduce manual effort.

---

## 🔧 Features

- 🧑‍⚕️ Doctor registration, login, and schedule management
- 🧑‍🦽 Patient registration, medical history, and record tracking
- 📅 Appointment booking system with availability check
- 💊 Prescription and diagnosis records
- 💵 Billing module with invoice generation
- 📊 Admin dashboard with CRUD operations for users and departments
- 🔐 Role-based authentication (Admin, Doctor, Patient)

---

## 🛠️ Tech Stack

### Backend:
- **Django** (Python Web Framework)
- **MySQL** (Relational Database)

### Frontend:
- HTML5, CSS3, JavaScript
- Bootstrap (for responsive design)

### Tools:
- VS Code
- Git & GitHub
- MySQL Workbench
- Postman (for API testing)

---

## 📁 Project Structure

```
HMS-Django/
├── hms/                    # Main project folder
│   ├── settings.py         # Django settings
│   ├── urls.py             # URL routing
│   └── wsgi.py
├── hospital/               # App containing core functionality
│   ├── models.py           # Database models
│   ├── views.py            # Business logic
│   ├── urls.py             # App-level routing
│   ├── templates/          # HTML templates
│   └── static/             # CSS, JS, and images
├── db.sqlite3 (if local) / mysql database
├── manage.py
├── requirements.txt
└── README.md
```

---

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/hms-django.git
cd hms-django
```

### 2. Create & Activate Virtual Environment

```bash
python -m venv env
source env/bin/activate   # On Windows use `env\Scripts\activate`
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Database

Update the `DATABASES` section in `hms/settings.py`:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'hms_db',
        'USER': 'your_mysql_user',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

Then apply migrations:

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create Superuser

```bash
python manage.py createsuperuser
```

### 6. Run Development Server

```bash
python manage.py runserver
```

Visit: `http://127.0.0.1:8000/`

---

## 🧪 Testing

- Use Django admin panel at `/admin`
- Test modules like:
  - Patient registration
  - Doctor schedule update
  - Appointment booking
  - Billing generation

---

## 🙋‍♂️ Team Member

- Vishali S — Developer & Project Lead

---

## 📜 License

This project is licensed under the MIT License. See `LICENSE` for more information.

---

## 📞 Contact

For queries or contributions, feel free to contact:

- VISHALI — [vishali.bm22@bitsathy.ac.in](mailto:vishali.bm22@bitsathy.ac.in)
