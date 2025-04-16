🔐 Django Authentication System with Email Service — Dockerized Microservices Architecture


<img width="1335" alt="Screenshot 2025-04-15 at 5 46 27 PM" src="https://github.com/user-attachments/assets/63783518-cc42-4c51-abdc-02cf223263c4" />

Django Authentication System with Email Service — Dockerized Microservices Architecture
A fully containerized Django authentication project built with Docker Compose. This project showcases how to structure and run multiple Docker containers for a modern, scalable web application — integrating services like PostgreSQL, Redis, and Celery for asynchronous email-based password reset functionality.

💡 Why This Project Stands Out
🔧 Key Feature: Docker Compose + Multi-Container Setup
This project is an excellent example of how to separate concerns using Docker Compose. Each service runs in its own container:

🐍 Django (Web App)

🐘 PostgreSQL (Database)

🔄 Redis (Broker for Celery)

⚙️ Celery (Asynchronous task runner for sending emails)

By leveraging Docker Compose, you can easily spin up the full development environment with one command, ensuring consistency across machines and teams.

🚀 Core Features
👤 User Registration & Login

🔁 Forgot Password – Email-based password reset

📩 Email Service – Secure email sending using App Passwords

🔒 Secure Profile Page

🛠️ Tech Stack
Django – Python web framework

PostgreSQL – Hosted relational DB

Celery + Redis – Async tasks for sending email

Docker & Docker Compose – Container orchestration

⚙️ How to Run (Using Docker Compose)
Set up Configuration

Update your email & database credentials in docker-compose.yml and settings.py.

Enable 2-Step Verification for your email, and use an App Password in place email password field in docker compose file .

Run All Containers


docker-compose up --build
This command builds and launches:

Django app container

PostgreSQL container

Redis container

Celery worker container

🔗 Access Your Project
After running the setup, open:

📍 http://localhost:8000/register

🧪 Quick Dev Tip
Use:


ALLOWED_HOSTS = ['*']
in settings.py to allow access from all hosts during development.
