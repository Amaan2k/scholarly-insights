# Scholarly Insights

A web application for discovering and discussing arXiv research papers.

## Team Members
- Aadarsh LN
- Amaan Ansari
- Julio Rodriguez
- Matthew Jiang
- Nitish KS
- Tanvi Takavane

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR-USERNAME/scholarly-insights.git
cd scholarly-insights
```

### 2. Backend Setup
```bash
cd backend
python3 -m venv venv

# Activate virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Create superuser (optional)
python manage.py createsuperuser

# Start server
python manage.py runserver
```

### 3. Frontend Setup
Open a new terminal:
```bash
cd frontend
npm install
npm start
```

### 4. Access the Application
- Backend API: http://127.0.0.1:8000/
- Django Admin: http://127.0.0.1:8000/admin/
- Frontend: http://localhost:3000/


## Project Structure
```
scholarly-insights/
├── backend/          # Django backend
│   ├── users/       # User management
│   ├── articles/    # Article CRUD and arXiv integration
│   ├── comments/    # Comment system
│   └── notifications/ # Notification system
└── frontend/         # React frontend
    └── src/
        ├── components/  # React components
        ├── pages/       # Page components
        └── services/    # API services
```

## Tech Stack
- **Frontend**: React
- **Backend**: Django + Django REST Framework
- **Database**: SQLite (development)
- **API Integration**: arXiv API

## Useful Commands

### Backend
```bash
# Create new app
python manage.py startapp app_name

# Make migrations
python manage.py makemigrations
python manage.py migrate

# Run tests
python manage.py test

# Access Django shell
python manage.py shell
```

### Frontend
```bash
# Install new package
npm install package-name

# Build for production
npm run build
```

## Getting Help
- Review Django docs: https://docs.djangoproject.com/
- Review React docs: https://react.dev/
