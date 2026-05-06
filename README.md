# 🛒 EcoMart - Professional E-Commerce Catalog

EcoMart is a fully functional, minimalist e-commerce platform built with **Django**. It features a dynamic product catalog, category filtering, a session-based shopping cart, and a complete checkout system.

## 🚀 Key Features

- **User Authentication:** Secure registration and login system for customers.
- **Product Catalog:** Dynamic grid display of products with high-quality image handling via **Pillow**.
- **SEO Optimized URLs:** Implementation of **Slugs** and `get_absolute_url` for professional, readable web addresses.
- **Advanced Search & Filtering:** Real-time search functionality and category-based filtering.
- **Session-Based Shopping Cart:** 
    - Add/Remove items without needing a database hit.
    - Persistent cart data during the user session.
    - Automatic total price calculation.
- **Checkout System:** Transactional order processing that converts cart sessions into permanent database records.
- **Responsive UI:** Clean, custom CSS with a focus on User Experience (UX) and template inheritance.

## 🛠️ Tech Stack

- **Backend:** Python 3.13+, Django 6.0+
- **Database:** SQLite (Relational)
- **Image Processing:** Pillow
- **Frontend:** HTML5, CSS3 (Custom Grid/Flexbox)
- **Version Control:** Git, GitHub

## 📦 Installation & Setup

1. **Clone the repository:**
```bash
git clone https://github.com/Obinna32/ecomart_project.git
cd ecomart_project
```

2. **Create a Virtual Environment**
```bash
python -m venv venv
#Windows
venv\Scripts\activate
#Mac/Linux:
source venv/bin/activate
```

3. **Install Dependencies**
```bash
pip install -r requirements.txt
```

4. **Database Setup**
```bash
python manage.py makemigrations
python manage.py migrate
```

5. **Run Server**:
```bash
python manage.py runserver
```

## 📐 Project Architecture
This project demonstrates several professional Django concepts:
* Context Processors: Making the cart available globally across all templates.
* Media Management: Configuring MEDIA_ROOT and MEDIA_URL for secure file uploads.
* Logic Separation: Moving complex cart logic into a standalone cart.py class to keep views clean.
* Relational Mapping: One-to-Many relationships between Categories, Products, and Orders



© 2026 EcoMart - Built by Obinna32 with Django