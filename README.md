# Flask Blog

> A modern blog application built with **Flask**, following best practices for authentication, database modeling, and web development. This project is part of my backend learning journey with Python.

---

## Features

- User registration with validation
- Secure login authentication
- Password hashing with Flask-Bcrypt
- User session management using Flask-Login
- SQLite database with SQLAlchemy ORM
- Responsive interface with Bootstrap
- User and Post database models
- Flash messages for user feedback
- Jinja2 template inheritance

---

## Tech Stack

- Python 3
- Flask
- Flask-SQLAlchemy
- Flask-WTF
- Flask-Bcrypt
- Flask-Login
- SQLite
- HTML5
- Bootstrap 5
- Jinja2

---

## Project Structure

```text
Flask_Blog/
│
├── flaskblog/
│   ├── static/
│   ├── templates/
│   ├── __init__.py
│   ├── forms.py
│   ├── models.py
│   └── routes.py
│
├── instance/
│   └── site.db
│
├── run.py
├── README.md
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/PedrReis-create/flask-course.git
```

Navigate to the project folder:

```bash
cd Flask_Blog
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it.

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python run.py
```

Open your browser and access:

```text
http://127.0.0.1:5000
```

---

## Current Features

- User registration
- Secure user authentication
- Password hashing
- Login persistence
- User and Post models
- One-to-many database relationship
- Responsive interface
- Flash messages
- Jinja2 template inheritance

---

## Planned Features

- Create posts
- Update posts
- Delete posts
- Upload profile pictures
- User profile page
- Pagination
- Password reset via email
- Authorization system
- Custom error pages
- Production deployment

---

## Database Models

### User

| Field | Type |
|------|------|
| id | Integer |
| username | String |
| email | String |
| image_file | String |
| password | String |

### Post

| Field | Type |
|------|------|
| id | Integer |
| title | String |
| content | Text |
| date_posted | DateTime |
| user_id | Foreign Key |

Relationship:

```text
User (1) ──────────── (*) Post
```

---

## Learning Goals

This project is part of my backend development journey. Through it, I am learning how to build secure web applications with Flask, work with relational databases using SQLAlchemy, implement user authentication, and organize scalable Python projects.

---

## Future Improvements

- Create, edit and delete blog posts
- User profile customization
- Profile picture uploads
- Password reset via email
- Pagination
- Custom error pages

---

## License

This project is licensed under the MIT License.