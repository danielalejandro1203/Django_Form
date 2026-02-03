# Job Application Form – Django

Simple Django web application that allows users to submit a job application
through a form. Submitted data is stored in a database and can be reviewed
through the Django Admin panel.

This project demonstrates core Django concepts such as forms, models,
views, ORM usage, messaging framework, and basic email notifications.

---

## Features

- Job application form with server-side validation
- Data storage using Django ORM
- Django Admin panel to view submitted applications
- Email confirmation sent after successful form submission
- CSRF protection
- Django messages framework for user feedback

---

## Tech Stack

- Python
- Django
- HTML
- Bootstrap
- SQLite

---

## How It Works

1. User fills out the job application form
2. Data is validated using Django Forms
3. Application data is saved to the database
4. Confirmation email is sent to the user
5. Admin users can view all submissions via Django Admin

---

## Installation & Setup

1. Clone the repository:

bash
git clone <repository-url>
cd <project-folder>

2. Create a virtual environment and activate it:
python -m venv venv
# macOS/Linux
source venv/bin/activate
# Windows
venv\Scripts\activate

3. Install dependencies:
pip install -r requirements.txt

4. Create the database and superuser: 
python manage.py migrate
python manage.py createsuperuser

Configuring Email (.env)

This project uses email notifications after a form submission.
To keep your credentials safe, email configuration is handled via a .env file.

1. In the root of the project, create a file called:
.env

2. Add your email credentials:
EMAIL_HOST_USER=your_email@gmail.com
EMAIL_HOST_PASSWORD=your_app_password

Running the project
python manage.py runserver
Access the form at: http://127.0.0.1:8000/
Access the admin panel at: http://127.0.0.1:8000/admin/ (login with superuser)

Purpose of the Project
This project was built to practice and demonstrate:

1. Django Forms
2. Models and ORM
3. Views and templates
4. Basic email handling
5. Admin interface usage
6. CSRF protection and messaging framework
