# 🚀 ToDo-Gemini: AI-Powered Task Management

A modern task management application powered by Google's Gemini AI, built with FastAPI and Python.

## 🌟 Features

- ✨ AI-powered task suggestions and organization
- 🔐 Secure user authentication
- 📱 Responsive web interface
- 🗄️ Database integration
- 🐳 Docker support for easy deployment
- 🔄 Database migrations with Alembic

## 🛠️ Tech Stack

- **Backend**: FastAPI
- **Database**: SQLite
- **AI Integration**: Google Gemini AI
- **Frontend**: HTML, CSS, JavaScript
- **ORM**: SQLAlchemy
- **Authentication**: JWT
- **Containerization**: Docker

## 📦 Installation

### Prerequisites

- Python 3.8+
- Docker and Docker Compose (optional)
- Google Gemini AI API key

### Local Installation

1. Clone the repository:
```bash
git clone https://github.com/tamerakdeniz/ToDo-Gemini.git
cd ToDo-Gemini
```

2. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
Create a `.env` file in the root directory with the following:
```
DATABASE_URL=postgresql://user:password@localhost:5432/todoai
SECRET_KEY=your-secret-key
GEMINI_API_KEY=your-gemini-api-key
```

### Docker Installation

1. Build and run with Docker Compose:
```bash
docker-compose up --build
```

## 🚀 How It Works

1. **User Authentication**
   - Register and login to access your personal task management space
   - Secure JWT-based authentication

2. **Task Management**
   - Create, read, update, and delete tasks
   - Organize tasks with categories and priorities
   - Set due dates and reminders

3. **AI Integration**
   - Get smart task suggestions based on your patterns
   - AI-powered task categorization
   - Natural language task processing

4. **Database**
   - Database for reliable data storage
   - Alembic migrations for database version control

## 🔧 Development

### Running the Application

```bash
uvicorn main:app --reload
```

### Running Tests

```bash
pytest
```

### Database Migrations

```bash
# Create a new migration
alembic revision --autogenerate -m "description"

# Apply migrations
alembic upgrade head
```


---

Made with ❤️ by [Your Name]
