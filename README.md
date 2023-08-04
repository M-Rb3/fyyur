# Fyyur - Venue Booking Site

![Python](https://img.shields.io/badge/python-3.9-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Database Setup](#database-setup)
- [Run the Application](#run-the-application)
- [License](#license)

## Introduction

Fyyur is a web application designed to help musicians and venue owners collaborate and book events. It's built using Flask, a popular Python web framework, and SQLAlchemy, a powerful SQL toolkit for Python. Fyyur allows artists to list their shows and receive booking requests from venue owners. Venue owners can browse through artist profiles and send booking offers.

## Features

- Artist and venue profiles with detailed information
- Browse upcoming shows and artists
- Venue owners can send booking offers to artists
- Manage and track booking requests
- Responsive and mobile-friendly design

## Requirements

- Python 3.9 or higher
- Flask (flask) web framework
- SQLAlchemy (sqlalchemy) SQL toolkit
- Flask-Migrate (flask-migrate) for database migrations
- WTForms (wtforms) library for form handling
- Flask-WTF (flask-wtf) for form validation
- PostgreSQL database (or any other supported by SQLAlchemy)

Install the required dependencies using the following command:

```bash
pip install -r requirements.txt
```

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/M-Rb3/fyyur.git
cd fyyur
```

2. Set up a virtual environment (optional but recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Database Setup

1. Create a PostgreSQL database for Fyyur. Make sure you have PostgreSQL installed.
2. Set the database URI in config.py to connect to your PostgreSQL database:

```python
SQLALCHEMY_DATABASE_URI = 'postgresql://username:password@localhost:5432/database_name'
```

Replace `username`, `password`, and `database_name` with your PostgreSQL credentials and database name.

3. Apply database migrations to create the necessary tables:

```bash
flask db upgrade
```

### Run the Application

1. Start the Flask development server:

```bash
export FLASK_APP=app.py
export FLASK_ENV=development
flask run
```

2. Open your web browser and visit http://localhost:5000 to access the Fyyur application.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
