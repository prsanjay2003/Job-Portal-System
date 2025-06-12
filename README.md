# Job Portal System

A web-based job portal system for job seekers and employers to connect, apply for jobs, and manage vacancies efficiently.

## Features
- User authentication (job seekers & employers)
- Job posting and application submission
- Profile management and resume upload
- Search and filtering options for job listings
- Employer dashboard for managing applications

## Installation Guide

### **1. Clone the Repository**
```
git clone <your-repo-url>
cd job-portal-system
```

### **2. Set Up the Database**
For MySQL (PHP-based systems):
1. Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
2. Create a new database: `job_portal_db`.
3. Import the provided `.sql` file.

For Firebase (Android-based systems):
1. Go to [Firebase Console](https://console.firebase.google.com/) and create a new project.
2. Enable Firestore Database or Realtime Database.
3. Add the `google-services.json` file inside the `app/` folder.

### **3. Configure Database Connection**
For PHP:
```php
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "job_portal_db";
```

For Firebase:
```python
import firebase_admin
from firebase_admin import credentials, firestore

cred = credentials.Certificate("path/to/google-services.json")
firebase_admin.initialize_app(cred)
db = firestore.client()
```

### **4. Run the Project**
For Web-based PHP System:
- Start **Apache** and **MySQL** in XAMPP.
- Open your browser and visit:
```
http://localhost/job-portal-system/
```

For Python-based System:
```
python app.py
```
If using Django or Flask:
```
python manage.py runserver
```

## How to Contribute
- Fork the repository
- Create a feature branch
- Make improvements
- Submit a pull request

## Author
Sanjay

## License
MIT License

```
