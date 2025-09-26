# DreamCache Website

DreamCache is a Django-based web application designed for journaling and personal thought management. Users can register, log in, create, update, and delete their thoughts, as well as manage their profiles. The project uses Django's built-in authentication system and provides a clean, user-friendly interface.

## Features

- User registration and authentication
- Create, view, update, and delete thoughts
- Profile management (including profile picture uploads)
- Password reset functionality
- Responsive design with custom CSS and JavaScript
- Admin interface for managing users and thoughts

## Project Structure

```
dreamcache-website/
│
├── db.sqlite3
├── manage.py
├── dreamcache/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── journal/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   ├── migrations/
│   └── templates/
│       └── journal/
│           ├── create-thought.html
│           ├── dashboard.html
│           ├── delete-account.html
│           ├── delete-thought.html
│           ├── index.html
│           ├── my-login.html
│           ├── my-thoughts.html
│           ├── navbar.html
│           ├── password-reset-complete.html
│           ├── password-reset-form.html
│           ├── password-reset-sent.html
│           ├── password-reset.html
│           ├── profile-management.html
│           ├── register.html
│           └── update-thought.html
│
├── media/
│   ├── default.png
│   ├── image1.jpg
│   └── paul-profile.jpg
│
└── static/
    ├── css/
    │   └── styles.css
    └── js/
        └── app.js
```

## Setup Instructions

1. **Clone the repository:**
   ```sh
   git clone <repository-url>
   cd dreamcache-website
   ```

2. **Create and activate a virtual environment:**
   ```sh
   python -m venv .venv
   .venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```sh
   pip install django
   ```

4. **Apply migrations:**
   ```sh
   python manage.py migrate
   ```

5. **Create a superuser (optional, for admin access):**
   ```sh
   python manage.py createsuperuser
   ```

6. **Run the development server:**
   ```sh
   python manage.py runserver
   ```

7. **Access the site:**
   - Open your browser and go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Customization

- **Static files:** Place your CSS and JS in `static/css/` and `static/js/`.
- **Media files:** User-uploaded files (like profile pictures) are stored in the `media/` directory.
- **Templates:** HTML templates are in `journal/templates/journal/`.


## License

This project is for educational and personal use. Please contact the author for other uses.

---

**Made with Django.**
