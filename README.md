# Flask Todo App

A simple Todo application built with Flask and SQLAlchemy for basic CRUD operations. This app allows you to create, read, update, and delete tasks.

## Features

- **Create**: Add new tasks with a title and description.
- **Read**: View all existing tasks.
- **Update**: Modify existing tasks.
- **Delete**: Remove tasks from the list.

## Requirements

- Python 3.x
- Flask
- Flask-SQLAlchemy
- PostgreSQL

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/SachiGaur14/Todo_app.git
cd your-repository-name
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the Database

Ensure you have PostgreSQL installed and running. Create a database named `flask_db` (or modify the database URI in `app.config` to match your database name).

### 5. Update the Database URI

Edit the `app.config['SQLALCHEMY_DATABASE_URI']` in `app.py` to match your PostgreSQL database credentials:

```python
app.config['SQLALCHEMY_DATABASE_URI'] = 'postgresql://username:password@localhost:5432/flask_db'
```

### 6. Initialize the Database

Run the following command to create the necessary tables:

```bash
python app.py
```

### 7. Run the Application

Start the Flask development server:

```bash
python app.py
```

Visit `http://127.0.0.1:5000/` in your browser to use the application.

## Project Structure

- `app.py`: Main application file containing routes and logic.
- `templates/`
  - `home.html`: Template for viewing and adding tasks.
  - `update.html`: Template for updating tasks.
- `requirements.txt`: Python package dependencies.

## Contributing

Feel free to submit pull requests or open issues if you encounter any problems or have suggestions for improvements.
