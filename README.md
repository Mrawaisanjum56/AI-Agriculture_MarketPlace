# AI-Agriculture_MarketPlace
It is a smart platform that connects farmers and buyers while using AI to analyze crop quality. The system uses deep learning (MobileNetV2) to classify crop images into quality categories, improving transparency in agricultural trade and enabling farmers to sell products directly in a digital marketplace.

# AI-Agriculture_MarketPlace— Django E-Commerce Platform

A university final year project built with **Django**, focused on an e-commerce workflow with custom user management, product/media handling, and optional machine-learning support for wheat quality grading.

## 📌 Project Overview

This project is a web-based e-commerce application developed as a final year university project by AWAIS ANJUM.  
It includes:

- User authentication with a custom user model
- Product/storefront flow
- Admin management via Django admin panel
- Media and static file handling
- SQLite-based data persistence
- Optional ML-assisted wheat quality grading (MobileNetV2/TensorFlow)
- Configurable AMIS scraping defaults for market-related data integration

---

## 🛠 Tech Stack

- **Backend:** Python, Django
- **Frontend:** HTML, CSS, SCSS, JavaScript
- **Database:** SQLite (`db.sqlite3`)
- **ML:** TensorFlow / Keras (MobileNetV2-based model support)

---

## 📂 Project Structure

```text
Final_project/
├── ecommers/              # Django project settings and root URL config
├── shop/                  # Main application (models, views, urls, auth logic)
├── templates/             # HTML templates
├── statics/               # Static assets (CSS/JS/images)
├── media/                 # Uploaded media files
├── models/                # ML model files (e.g., wheat_quality.keras)
├── assets/                # Additional project assets
├── manage.py              # Django management entry point
├── db.sqlite3             # SQLite database
└── README.md
```

---

## ✅ Requirements

### 1) System Requirements
- Python **3.10+** (recommended)
- pip (latest)
- Git
- Virtual environment tool (`venv`)

### 2) Python/Django Requirements
- Django **6.0** (project generated with Django 6.0)
- Pillow (recommended for image handling)
- TensorFlow ( for wheat quality model)

### 3) ML Requirement
If you want ML-based wheat grading:

```bash
pip install tensorflow
```

If TensorFlow is not installed, the project can fall back to a lightweight heuristic flow (as noted in project behavior).

### 4) Environment Variables (Recommended)
Create environment variables for sensitive/configurable values:

- `DJANGO_SECRET_KEY`
- `AMIS_BASE_URL`
- `AMIS_MARKET_FILTER`
- `AMIS_SCRAPE_TIMEOUT`
- `EMAIL_HOST_USER`
- `EMAIL_HOST_PASSWORD`

---

## 🚀 Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/Mrawaisanjum56/AI-Agriculture_MarketPlace.git
cd Final_project
```

### 2. Create and activate virtual environment
**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt

pip install django pillow
pip install tensorflow
```

### 4. Apply migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create superuser (optional but recommended)
```bash
python manage.py createsuperuser
```

### 6. Run development server
```bash
python manage.py runserver
```

Open: `http://127.0.0.1:8000/`

---


---

## 🌐 Main Routes

- `/` → Shop app routes (via `shop.urls`)
- `/admin/` → Django admin panel

---

## 🧪 Suggested Future Improvements

- Add unit/integration tests
- Add CI workflow (GitHub Actions)
- Configure production server (Gunicorn + Nginx + PostgreSQL)
- Add Docker support

---

## 👨‍🎓 Academic Context

This repository is developed as a **University Final Year Project**, demonstrating full-stack web development with Django and practical integration of domain-specific logic.

-

---

## 🤝 Author

**Awais Anjum**  
GitHub: [@Mrawaisanjum56](https://github.com/Mrawaisanjum56)