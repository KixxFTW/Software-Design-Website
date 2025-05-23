# UCU+ Merchandise Hub

A Flask web application for managing UCU's merchandise store, student dashboard, and payment system.

## Table of Contents
  - [Features](#features)
  - [Quick Start](#quick-start)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
  - [Running the Application](#running-the-application)
  - [Project Structure](#project-structure)
  - [Contributing](#contributing)
  - [Admin](#Admin)
  - [Dependencies and Libraries](#dependencies-and-libraries)

## Features

### Authentication
  - Student/Instructor Authentication (Email + Google OAuth)
  - Role-based access control

### Student Dashboard
  - Course enrollment information
  - Academic calendar
  - Grades overview
  - Department merchandise shopping

### E-commerce
  - Shopping Cart System
  - Payment Processing
  - Order tracking

### Administration
  - Admin Panel for managing products
  - Order management
  - User management

## Quick Start

To get started quickly:

```bash
cd "C:\Users\valde\Flowers\website\UCU+ Software Design"
python run.py
```

## Prerequisites

- Python 3.8+
- MySQL 8.0+
- pip (Python package manager)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd ucu-merch-hub
```

2. Create and activate virtual environment:
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Unix/MacOS:
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Configuration

1. Database Setup:
   - Create a MySQL database named 'ucu_merch'
   - Update database settings in `config.py`

2. Environment Variables:
   Create a `.env` file with:
   ```
   SECRET_KEY=your-secret-key
   MYSQL_HOST=localhost
   MYSQL_USER=your-username
   MYSQL_PASSWORD=your-password
   MYSQL_DB=ucu_merch
   GOOGLE_CLIENT_ID=your-google-client-id
   GOOGLE_CLIENT_SECRET=your-google-client-secret
   ```

## Running the Application

1. Initialize the database:
```bash
flask db init
flask db migrate
flask db upgrade
```

2. Start the development server:
```bash
python run.py
```

The application will be available at `http://127.0.0.1:5000`

## Project Structure

```
ucu-merch-hub/
├── app/
│   ├── templates/       # HTML templates
│   ├── static/          # Static files
├── requirements.txt     # Project dependencies
└── run.py              # Application entry point
```

## Contributing

1. Fork the repository
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Create a Pull Request

## Admin Panel
STUDENT ID--ADMIN001
PASSWORD - admin123

## Dependencies and Libraries

### Core Framework
- Flask (Web framework)
- Werkzeug (WSGI web application library)
- Jinja2 (Template engine)

### Database
- MySQL Connector Python (Database interface)
- Flask-MySQL (Flask extension for MySQL)
- Flask-SQLAlchemy (SQL ORM)
- Flask-Migrate (Database migrations)

### Authentication & Security
- Flask-Login (User session management)
- Flask-Bcrypt (Password hashing)
- Flask-OAuth (OAuth integration)
- Google OAuth2 (Google authentication)
- PyJWT (JSON Web Tokens)

### Frontend
- Material Design Icons
- Bootstrap (via CDN)
- jQuery (via CDN)
- Google Fonts (Roboto, Ubuntu)

### Payment Processing
- **GCash** (Philippine mobile wallet integration)
- **Maya** (Philippine digital wallet integration)
- **Bank Transfer** (Manual or API-based bank payments)

### Utilities
- python-dotenv (Environment variables)
- Flask-Mail (Email functionality)
- Pillow (Image processing)
- Flask-WTF (Form handling)
- email-validator (Email validation)
- requests (HTTP requests)
- oauthlib (OAuth support)
- requests-oauthlib (OAuth for requests)

### Development Tools
- Flask-DebugToolbar
- python-dateutil
- pytz (Timezone handling)

### System Requirements
- Python 3.8+
- MySQL 8.0+
- pip (Python package manager)

To install all dependencies:
```bash
pip install -r requirements.txt
```

## Backend Tools

- Flask (Web framework)
- Werkzeug (WSGI web application library)
- Jinja2 (Template engine)
- Flask-MySQL (Flask extension for MySQL)
- MySQL Connector Python (Database interface)
- Flask-SQLAlchemy (SQL ORM)
- Flask-Migrate (Database migrations)
- Flask-Login (User session management)
- Flask-Bcrypt (Password hashing)
- Flask-OAuth (OAuth integration)
- Google OAuth2 (Google authentication)
- PyJWT (JSON Web Tokens)
- python-dotenv (Environment variables)
- Flask-Mail (Email functionality)
- Pillow (Image processing)
- Flask-WTF (Form handling)
- email-validator (Email validation)
- requests (HTTP requests)
- oauthlib (OAuth support)
- requests-oauthlib (OAuth for requests)
- Flask-DebugToolbar (Debugging)
- python-dateutil (Date/time utilities)
- pytz (Timezone handling)

## Frontend Tools

- Jinja2 (Template engine for dynamic HTML)
- Bootstrap (CSS framework, via CDN)
- Material Design Icons (Icon font, via CDN)
- jQuery (JavaScript library, via CDN)
- Google Fonts (Roboto, Ubuntu)
- Custom CSS/JS (in your static/ directory)