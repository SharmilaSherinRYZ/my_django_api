# 🏥 Patient Management System API (FastAPI + Docker)

This project is a **RESTful API** built using **FastAPI** to manage and access **patient records** stored in a local JSON file (`patients.json`).

---

## 🚀 Features

- ✅ View a welcome/home message
- ✅ Learn about the API from an `/about` route
- ✅ View all patient records
- ✅ Get details of a specific patient using their ID
- ✅ Sort patients based on `height`, `weight`, or `bmi` (Body Mass Index)

---

## 📁 Project Structure

fast_api_project/
├── main.py ← FastAPI app
├── patients.json ← Patient data in JSON format
├── requirements.txt ← Python dependencies
├── Dockerfile ← For Docker image

yaml
Copy
Edit

---

## 📦 Technologies Used

- **FastAPI** – Web framework for building APIs quickly
- **Python 3.11+**
- **Docker** – To containerize and run the app easily
- **JSON** – Used as a simple database

---

## ▶️ How to Run the App Locally

### 🐳 Using Docker

1. Clone this repo  
2. Make sure `patients.json` is in the same folder as `main.py`
3. Build the Docker image:
     ```bash
        docker build -t patient-api .
4. Run the container:

    ```bash
       docker run -d -p 8000:8000 patient-api
### Open in browser:

Home: http://localhost:8000

API Docs: http://localhost:8000/docs

### 📚 API Endpoints
Method	Endpoint	Description
GET	/	Welcome message
GET	/about	Info about the project
GET	/view	View all patient records
GET	/patient/{patient_id}	View details of a patient by ID
GET	/sort	Sort patients by height, weight, or bmi

### 🧪 Example: Get a patient by ID

```bash
GET /patient/P001
Returns details of patient with ID P001.

### 🧠 How It Works
All patient records are stored in a JSON file.

When you call an endpoint:

The file is read

The requested data is retrieved, filtered, or sorted

The result is returned as a JSON response

#### 💡 Sample patients.json Structure
```bash
{
  "P001": {
    "name": "John Doe",
    "age": 45,
    "height": 175,
    "weight": 80,
    "bmi": 26.1
  },
  "P002": {
    "name": "Jane Smith",
    "age": 30,
    "height": 160,
    "weight": 60,
    "bmi": 23.4
  }
}