# Django Blog Application

This is a simple Django-based blog application that includes basic features like viewing blog posts, category management, and an admin interface.

# Project Structure

MYAPP/
├── blog/
│ ├── init.py
│ ├── admin.py
│ ├── apps.py
│ ├── form.py
│ ├── models.py
│ ├── tests.py
│ ├── urls.py
│ ├── templates/
│ │ ├── about.html
│ │ ├── contact.html
│ │ ├── detail.html
│ │ ├── index.html
│ ├── migrations/
│ ├── static/
│ ├── management/
│ │ ├── commands/
│ │ │ ├── init.py
│ │ │ ├── populate_category.py
│ │ │ └── populate_data.py

## Features

- Blog post listing and detail view
- Static and template file support
- Management commands for populating data and categories
- Admin interface for managing models

## Setup Instructions

# step1: Clone the Repository

   ```bash
   git clone <repository_url>
   cd MYAPP

# Step 2: Create a virtual environment
python -m venv venv && \

# Step 3: Activate the virtual environment (use appropriate command for your OS)
source venv/bin/activate && \  # For macOS/Linux
# venv\Scripts\activate && \   # For Windows (uncomment and use this line instead)

# Step 4: Install project dependencies
pip install -r requirements.txt && \

# Step 5: Apply database migrations
python manage.py migrate && \

# Step 6: Populate categories (custom management command)
python manage.py populate_category && \

# Step 6 (continued): Populate blog data (custom management command)
python manage.py populate_data && \

# Step 7: Run the development server
python manage.py runserver
