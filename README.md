# CustTweet 🐦  
A simple Twitter-like application built with **Django**, where users can register, log in, and create, edit, and delete tweets.  

---
<img width="926" height="532" alt="image" src="https://github.com/user-attachments/assets/a26c31ea-7126-45b3-adf4-8ea3a7e9ee71" />
<img width="1352" height="605" alt="image" src="https://github.com/user-attachments/assets/a323d31b-9251-49e2-bc34-0bd670e74fb1" />
<img width="1211" height="592" alt="image" src="https://github.com/user-attachments/assets/bbcfdd22-2d3f-4cd1-abec-8d454ee87e21" />
<img width="875" height="608" alt="image" src="https://github.com/user-attachments/assets/8bbaca7d-0247-4398-a63c-17b80420c7ea" />

## 🚀 Features
- User authentication (Register, Login, Logout).  
- Create tweets with text and optional file uploads.  
- Edit or delete only your own tweets.  
- View all tweets in a feed (sorted by newest first).  
- Basic media & static file support.  

---

## 📂 Project Structure  

```
CustTweet/
│── CustTweet/              # Project settings
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│
│── media/                  # Uploaded files
│── static/                 # Static files (CSS, JS, images)
│── templates/              # Global templates (base.html, index.html, etc.)
│
│── tweet/                  # Main app
│   ├── migrations/         
│   ├── templates/          # App-specific templates
│   │   └── tweet_list.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
│
│── db.sqlite3              # Default SQLite database
│── manage.py               # Django project manager
│── requirements.txt        # Project dependencies
│
└── myvenv/                 # Virtual environment
```

---

## ⚙️ Installation & Setup  

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/yourusername/custtweet.git
cd custtweet
```

### 2️⃣ Create and activate a virtual environment  
```bash
python -m venv myvenv
source myvenv/bin/activate   # On macOS/Linux
myvenv\Scripts\activate      # On Windows
```

### 3️⃣ Install dependencies  
```bash
pip install -r requirements.txt
```

### 4️⃣ Apply migrations  
```bash
python manage.py migrate
```

### 5️⃣ Create a superuser (optional, for admin access)  
```bash
python manage.py createsuperuser
```

### 6️⃣ Run the development server  
```bash
python manage.py runserver
```
Visit **http://127.0.0.1:8000/** 🎉  

---

## 🖥️ Usage  

- **Home Page** → `/`  
- **Tweet Feed** → `/tweets/`  
- **Create Tweet** → `/tweets/create/`  
- **Edit Tweet** → `/tweets/edit/<id>/`  
- **Delete Tweet** → `/tweets/delete/<id>/`  
- **Register** → `/register/`  
- **Login/Logout** → Django’s built-in auth views  

---

## 🛠️ Tech Stack
- **Backend**: Django (Python)  
- **Database**: SQLite (default, can be swapped for PostgreSQL/MySQL)  
- **Frontend**: Django Templates (HTML, CSS)  

---

## 📜 License
This project is licensed under the MIT License.  

---

👉 Next step: I can generate a **requirements.txt** file tailored to your project (with Django and any other needed packages).  
Do you want me to create that for you automatically?
