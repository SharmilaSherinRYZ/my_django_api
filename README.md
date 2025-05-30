# 🛍️ Product API (Django REST Framework + Docker)

This project is a **RESTful API web service** built using Django and Django REST Framework to manage products.  
Each product includes an `id`, `name`, and `price`. You can **create**, **retrieve**, **update**, and **delete** products through simple API calls.

---

## 📦 Features

- CRUD API for product data
- Built with Django REST Framework
- Dockerized for easy setup and portability
- No database configuration needed (uses Django defaults)
- Lightweight and beginner-friendly

---

## 🚀 How to Run Locally (Dockerized)

### 🛠️ Prerequisites

- [Docker](https://www.docker.com/) installed
- [Git](https://git-scm.com/) installed

### 📥 Steps to Run

1. **Clone the repository**
```bash
git clone https://github.com/SharmilaSherinRYZ/my_django_api.git
cd my_django_api

2. **Build and run using Docker**
```bash
docker-compose up --build

3. **Access the API**

Base URL: `http://localhost:8000/api/products/`

## 🔄 API Endpoints (Supported)

| Method | Endpoint         | Description           |
|--------|------------------|-----------------------|
| GET    | `/api/products/` | Retrieve all products |
| POST   | `/api/products/` | Create a new product  |

📌 **Example JSON for POST:**

```json
{
  "name": "Computer",
  "price": 100000.0
}

## 👨‍💻 Tech Stack

- Python 3.x  
- Django 4.x  
- Django REST Framework  
- Docker

