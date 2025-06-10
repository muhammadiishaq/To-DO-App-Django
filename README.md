# Django To-Do App

A simple yet powerful **To-Do App** built with Django, featuring a **CI/CD pipeline** using Jenkins, GitHub, and Docker for automated deployment.

![To-Do App](https://raw.githubusercontent.com/shreys7/django-todo/develop/staticfiles/todoapp.png)

## 🚀 Features
- Add, update, and delete tasks effortlessly.
- User authentication for secure access.
- Integrated **CI/CD pipeline** with **Jenkins & GitHub Webhooks**.
- Dockerized application for seamless deployment.
- Automatic builds, testing, and deployment on each GitHub commit.

## 🛠️ Installation
To set up the project locally, follow these steps:

### Clone the Repository
```bash
$ git clone https://github.com/yourusername/django-todo.git
$ cd django-todo
```

### Create a Virtual Environment
```bash
$ python -m venv venv
$ source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### Install Dependencies
```bash
$ pip install -r requirements.txt
```

### Apply Database Migrations
```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

### Create a Superuser (Admin)
```bash
$ python manage.py createsuperuser
```

### Run the Development Server
```bash
$ python manage.py runserver
```
Access the app at: **http://127.0.0.1:8000/todos**

## 📦 Docker Setup
To run the app in a Docker container:
```bash
$ docker build -t django-todo .
$ docker run -p 8000:8000 django-todo
```

## 🔄 CI/CD Pipeline (Jenkins & GitHub)
This project features an automated deployment pipeline:
1. Push changes to **GitHub**
2. **Jenkins Webhook** triggers an automated build
3. **Docker container** gets rebuilt and deployed

## 🎯 Tech Stack
- **Django** (Backend)
- **SQLite/PostgreSQL** (Database)
- **Jenkins** (CI/CD Automation)
- **Docker** (Containerization)
- **GitHub Webhooks** (Automated Deployment)

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
**Happy Coding! 🚀**

