# Flask CRUD Application

A simple CRUD (Create, Read, Update, Delete) web application built with Flask, SQLite, and Bootstrap. This application allows users to manage a list of students with attributes like first name, last name, email, gender, hobbies, and country.

## Features

- **Create**: Add new students with details such as first name, last name, email, password, gender, hobbies, and country.
- **Read**: View a list of all students in a formatted table.
- **Update**: Edit student details.
- **Delete**: Remove a student from the list.
- **User-Friendly UI**: Responsive design using Bootstrap.

## Tech Stack

- **Backend**: Flask (Python)
- **Database**: SQLite
- **Frontend**: HTML, CSS, Bootstrap
- **Templating**: Jinja2 for HTML templating with Flask

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/bhavesh-mbyte/my-flask-crud-app.git
cd my-flask-crud-app
```
### 2. Set Up a Virtual Environment

It’s recommended to use a virtual environment for project dependencies:
```bash
python -m venv venv
# On Windows use:
venv\Scripts\activate
# On macOS/Linux use:
source venv/bin/activate
```
### 3. Install Requirements

Install the required Python packages:
```bash
pip install -r requirements.txt
```
### 4. Run the Application

Initialize the SQLite database and run the Flask application:
```bash
# Set up environment variable
export FLASK_APP=app.py  # On Windows use: set FLASK_APP=app.py

# Create the database tables
flask shell
from models import db
db.create_all()
exit()

# Run the application
flask run
```
### 5. Access the Application

Once the server is running, open a browser and go to:
http://127.0.0.1:5000/

###  Project Structure

```bash
my-flask-crud-app/
├── app.py                # Main application file
├── models.py             # Database model file
├── templates/            # HTML templates
│   ├── master.html
│   ├── create.html
│   ├── update.html
│   ├── delete.html
│   └── index.html
├── requirements.txt      # Python dependencies
└── README.md             # Project readme file
```
