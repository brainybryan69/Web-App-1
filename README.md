# Full-Stack Web Application

A web application built with React frontend and Django backend, featuring user authentication and note management functionality.

## Tech Stack

**Frontend:**
- React 19.1.1
- JavaScript/JSX
- React Router DOM
- Vite (build tool)
- Axios for API calls
- Custom CSS

**Backend:**
- Python 3.13
- Django 5.2.5
- Django REST Framework
- PostgreSQL database
- JWT authentication
- CORS support

**Development Tools:**
- ESLint
- Git version control
- Python virtual environment
- Choreo deployment

## Features

- User registration and login
- JWT token authentication
- Protected routes
- Note creation and management
- Responsive design
- Loading indicators

## Project Structure

```
Web-App-1/
├── frontend/           # React app
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── styles/
│   │   └── api.js
│   └── package.json
├── backend/           # Django app
│   ├── api/
│   ├── backend/
│   ├── requirements.txt
│   └── manage.py
```

## Setup

### Backend
```bash
cd backend
python -m venv env
source env/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Frontend
```bash
cd frontend
npm install
npm run dev
```

## Environment Variables

**Backend (.env):**
```
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_HOST=localhost
DB_PORT=5432
```

**Frontend (.env):**
```
VITE_API_URL=http://127.0.0.1:8000
```

## API Endpoints

- `POST /api/users/register/` - User registration
- `POST /api/token/` - User login
- `GET /api/notes/` - Get user notes
- `POST /api/notes/` - Create note
- `DELETE /api/notes/{id}/` - Delete note

## Skills Used

- Frontend: React, JavaScript, CSS, responsive design
- Backend: Python, Django, REST APIs, database design
- Authentication: JWT tokens, protected routes
- Database: PostgreSQL, data modeling
- Deployment: Cloud platforms, environment configuration
- Tools: Git, npm, pip, virtual environments