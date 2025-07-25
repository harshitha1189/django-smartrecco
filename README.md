
# Django-SmartRecco Backend

This is the backend of the **SmartRecco** project — built with Django and focused on user authentication via Django REST Framework.

---

## 🔐 Features

- User registration
- Login with JWT/token authentication
- Secure password hashing
- User profile management
- Django REST Framework-based API

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/harshitha1189/django-smartrecco.git
cd django-smartrecco
````

### 2. Create virtual environment & install dependencies

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Set up environment variables

Create a `.env` file or set values in `settings.py`:

```env
SECRET_KEY=your_secret_key
DEBUG=True
```

### 4. Run migrations and start server

```bash
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

---

## 📬 API Endpoints

| Method | Endpoint         | Description         |
| ------ | ---------------- | ------------------- |
| POST   | `/api/register/` | Register a new user |
| POST   | `/api/login/`    | Login and get token |
| GET    | `/api/user/`     | Get user profile    |
| PUT    | `/api/user/`     | Update user profile |

> Auth is typically handled via JWT or token in headers:

```
Authorization: Token <your_token_here>
```

---

## 📁 Project Structure

```
smartrecco-backend/
├── authentication/         # Custom auth app
├── smartrecco_backend/     # Django project settings
├── manage.py
└── requirements.txt
```

---

## 🧪 Testing

To run tests (if you have them set up):

```bash
python manage.py test
```

---

## 📃 License

MIT — do what you want, just give credit.

---

## 🙋‍♀️ Maintainer

Created and maintained by **Harshitha**
Feel free to reach out via [GitHub](https://github.com/harshitha1189)

````

---

Let me know if you’re using JWT or just Django's default token system — I can tweak the examples accordingly. Once this looks good to you, save it as `README.md` in your project root, commit it:

```bash
git add README.md
git commit -m "Add README"
git push
````
