# Django Blog App

## Introduction

This project is a simple blog application built using Django, a powerful web framework for Python. The blog allows users to create, edit, and delete posts. It includes user authentication for post creation and comment functionality.

## Features

1. **User Authentication:**
   - Users can sign up, log in, and log out.
   - Only authenticated users can create, edit, and delete posts.
   
2. **Post Management:**
   - Authenticated users can create, edit, and delete their blog posts.
   - Each post contains a title, content, and publication date.

3. **Comment System:**
   - Users can leave comments on blog posts.
   - Comment authors are displayed with their usernames and timestamps.

## Setting Up the Project

### Prerequisites

- Python installed on your machine
- Django framework installed (`pip install django`)

### Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/samagra44/django-blog-app.git
   ```

2. **Navigate to Project Directory:**
   ```bash
   cd django-blog-app
   ```

3. **Create and Apply Migrations:**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

4. **Create a Superuser Account:**
   ```bash
   python manage.py createsuperuser
   ```

   Follow the prompts to create a superuser account. This account will have administrative access to the Django admin panel.

5. **Run the Development Server:**
   ```bash
   python manage.py runserver
   ```

6. **Access the Application:**
   Open your web browser and go to [http://localhost:8000/](http://localhost:8000/) to access the blog application.

7. **Access the Admin Panel:**
   Navigate to [http://localhost:8000/admin/](http://localhost:8000/admin/) and log in with the superuser credentials created earlier. Here, you can manage users, posts, and comments.

## Project Structure

The project follows a typical Django project structure with additional directories for templates and static files. The main components include:

- **Blog App (`blog`):**
  - Models define the structure of blog posts and comments.
  - Views handle the logic for displaying posts, creating, editing, and deleting posts, and managing comments.
  - Templates contain HTML files for rendering pages.

- **User Authentication (`accounts`):**
  - Handles user registration, login, and logout.
  - Utilizes Django's built-in authentication system.

- **Django Admin Panel:**
  - Accessible at [http://localhost:8000/admin/](http://localhost:8000/admin/) for managing users, posts, and comments.

Feel free to explore and customize the project based on your preferences. You can extend the functionality by adding features such as tags, categories, or user profiles.
