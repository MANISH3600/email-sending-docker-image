🔐 Simple Django Authentication Project
This is a basic authentication service built with Django. It includes:

User registration

User login

A profile page

Forgot password functionality — if the user exists in the database, they'll receive a reset email like this:

<img width="1335" alt="Screenshot 2025-04-15 at 5 46 27 PM" src="https://github.com/user-attachments/assets/63783518-cc42-4c51-abdc-02cf223263c4" />

🛠️ Technologies Used
Django

Redis

Celery

PostgreSQL (hosted online)

Docker & Docker Compose

⚙️ Setup Instructions
Update your settings in docker-compose file :

Enter your PostgreSQL database credentials .

Enter your email address (used to send reset links).

Enable 2-Step Verification for your email and use the App Password (paste it without any spaces).

Run the project:

In the project’s root directory (where manage.py is located), run:


docker-compose up --build
This will build and run all containers defined in docker-compose.yml and Dockerfile.

✅ After Setup
Once the containers are up, access the project at:


http://localhost:8000/register
🧪 Development Tip
For testing purposes, you can use:


ALLOWED_HOSTS = ['*']
in your settings.py to allow all hosts.

That’s it — no extra steps needed!
