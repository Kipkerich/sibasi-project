
# 📝 Django To-Do & Cards App

A responsive Django web application with a built-in user authentication system. After logging in, users can access a simple to-do list (without database persistence) and a second page containing styled text cards.

---

## 🚀 Features

- 🔐 User Signup, Login, and Logout
- ✅ Protected routes using `@login_required`
- 🏠 Home page with a non-database to-do list (client-side only)
- 📇 Cards page displaying responsive text cards
- 📱 Fully responsive UI with basic CSS (mobile-first)
- 🧩 Built using Django (Python Web Framework)

---

## 🧰 Technologies Used

- Python 
- Django 
- HTML5, CSS3
- JavaScript 
- Bootstrap

---

## 🗂️ Project Structure

```
mysite/
│
├── main/
│   ├── migrations/
│   ├── templates/
│   │   ├── base.html
│   │   ├── home.html
│   │   ├── cards.html
│   │   ├── login.html
│   │   └── signup.html
│   ├── urls.py
│   └── views.py
│
├── static/              
├── mysite/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── manage.py
```

---

## ⚙️ Installation & Setup

1. **Clone the repository**

```bash
git clone https://github.com/Kipkerich/sibasi-project.git
cd django-todo-cards
```

2. **Create and activate a virtual environment**

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**

```bash
pip install django
```

4. **Run migrations**

```bash
python manage.py makemigrations
python manage.py migrate
```

5. **Create a superuser (optional)**

```bash
python manage.py createsuperuser
```

6. **Run the development server**

```bash
python manage.py runserver
```

---

## 🔐 Authentication Redirects

In `settings.py`, these settings ensure smooth authentication flow:

```python
LOGIN_URL = '/login/'
LOGIN_REDIRECT_URL = '/'
LOGOUT_REDIRECT_URL = '/login/'
```

---



## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 💡 Future Improvements

- Save to-do items in the database
- Use Bootstrap or Tailwind for UI enhancements


---

## ✨ Author

Developed by [Kipkerich](https://github.com/Kipkerich)

