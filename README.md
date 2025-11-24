# Python URL Shortener

A simple and efficient **URL Shortener web application** built using **Flask** and **SQLite**.  
It allows users to convert long URLs into short codes, track visit counts, and delete shortened URLs.

---

## Features

- Shorten long URLs instantly  
- Auto-generated 6-character shortcode  
- Redirect to original URL  
- Track number of visits  
- Delete any short URL  
- Simple and clean UI (TailwindCSS)  
- Lightweight SQLite database  
- Backend functions:
  - `insert_url(originalURL, short_code)`
  - `get_url(short_code)`
  - `increment_visit_code(short_code)`
  - `get_all_url()`
  - `delete_url_by_code(short_code)`

---

## Tech Stack

| Component | Technology |
|----------|------------|
| Backend  | Flask (Python) |
| Database | SQLite |
| Frontend | HTML, TailwindCSS |
| Language | Python 3 |

---

## Project Structure

```
URL-Shortener/
│
├── app.py
├── models.py
├── database.db
├── requirements.txt
├── templates/
│   ├── index.html
│   └── 404.html
└── readme.txt
```

---

## Installation & Setup

### **1️ Create Python Virtual Environment**
```bash
python -m venv venv
```

### **2️ Activate the Virtual Environment**

#### Windows:
```bash
venv\Scripts\activate
```

#### macOS / Linux:
```bash
source venv/bin/activate
```

---

### **3️ Install Required Libraries**
```bash
pip install -r requirements.txt
```

If Flask is missing:
```bash
pip install flask
```

---

### **4 Run the Application**
```bash
python app.py
```

Server runs at:
```
http://localhost:8000
```

---

## How It Works

- User enters a long URL  
- Backend generates a **6-character shortcode**  
- Data saved into SQLite  
- Redirect increases visit count  
- URL list shows delete options  

---

## Developer
Abhijeet
