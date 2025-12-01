
# 🎬 Movie Project — Django + Django REST Framework

A full-stack movie platform built with **Django** and **Django REST Framework**, featuring both a **REST API** and a **Django web interface**.  
This project allows users to browse movies, view details, and interact with film-related content through API endpoints or the website.

---

## 🚀 Features

### 🔹 **Backend (API)**
- CRUD operations for movies  
- JWT authentication (login/register)  
- Movie categories & genres  
- Pagination & filtering  
- Fully RESTful API built using DRF  
- Clean, scalable project architecture  

### 🔹 **Frontend (Django Web)**
- Classic Django website  
- Movie list and detail pages  
- Admin panel for managing content  
- Template-based UI  

---

## 🛠️ Tech Stack

**Backend**
- Python  
- Django  
- Django REST Framework  
- PostgreSQL  

**Other**
- JWT Authentication  
- Docker-ready architecture (optional)  

---

## 📁 Project Structure



movie_project/
│
├── api/              # REST API app (movies, auth, serializers, views)
├── web/              # Django web app (templates, user interface)
├── movie_project/    # Core project settings
└── requirements.txt  # Dependencies


---

## 🔑 API Endpoints (Examples)

### Auth


POST /api/auth/register/
POST /api/auth/login/



### Movies


GET    /api/movies/
GET    /api/movies/<id>/
POST   /api/movies/
PUT    /api/movies/<id>/
DELETE /api/movies/<id>/


---

## ▶️ Installation

Clone the project:


git clone https://github.com/A1isherDev/movie_project.git
cd movie_project


Create a virtual environment:


python3 -m venv venv
source venv/bin/activate


Install dependencies:


pip install -r requirements.txt


Apply migrations:


python manage.py migrate


Run the server:


python manage.py runserver


---

## 🔐 JWT Authentication

To get tokens:


POST /api/auth/login/


Response:


{
  "refresh": "your_refresh_token",
  "access": "your_access_token"
}

Use the **access token** in headers:

Authorization: Bearer <token>


---

## 🌐 Deployment (General Guide)

1. Set up a VPS
2. Install Python + PostgreSQL
3. Configure Gunicorn + Nginx
4. Run Django backend on a service
5. Serve static files
6. Add free domain or `.uz` domain

If you want, I can generate a full **deployment guide** for this project too.

---

## 📜 License

This project is open-source. You may modify or reuse it freely.

---

## 👨‍💻 Author

**Alisher (@A1isherDev)** — Backend Developer (Python, Django, DRF)



---
