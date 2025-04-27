# Educa - E-Learning Platform

Educa is an online learning platform built with Django.

## Features

- **Authentication**: User Registration, Login, Logout
- **Course Management**:
  - Instructors can create, update, and delete courses
  - Organize courses into modules and multiple types of content (Text, Files, Images, Videos)
- **Student Enrollment**:
  - Students can browse and enroll in courses
  - Access enrolled course materials
- **Real-Time Messaging**:
  - Chat functionality using Django Channels and WebSockets
  - Redis used as the channel layer backend
- **REST API**:
  - Exposes course data with Django REST Framework


## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/HachemiIbrahim/educa.git
cd educa
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

### 3. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 4. Pull and Run Redis (Required for Channels)

If you have Docker installed:

```bash
docker run -it --rm --name redis -p 6379:6379 redis
```
### 5. Run Database Migrations

```bash
python manage.py migrate
```

### 6. Run the Development Server

```bash
python manage.py runserver
```

Visit:

```
http://127.0.0.1:8000/
```
