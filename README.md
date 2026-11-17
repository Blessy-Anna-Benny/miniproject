 Placement Statistics Website

 📌 Project Overview

A Django web application that helps engineering students view placement-related information and estimate their chances of being placed. Students register with their academic details, and a machine learning model predicts placement probability from CGPA, MOOC courses and internships.

The application integrates backend functionality, database management, and data-driven analysis within a centralized web platform.

 ✨ Key Features

* Student registration and login: A custom Django user model (UserRegistration) stores username, email, department, registration and admission numbers, CGPA, year, semester, HSC and SSLC scores, MOOC course, internships and phone number.
* Placement probability prediction: Students enter CGPA, number of MOOC courses and number of internships, and receive a Placed / Not Placed result with the probability of each outcome.
* Placement data display: Administrators upload Excel files (.xls / .xlsx) through the Django admin, and the site reads them with Pandas and shows them as tables.
* Events and notifications: Administrators add events and trainings in the admin panel. Students see them on the Events page and on a Notifications page sorted by newest first.
* Account management: Login, logout and change-password pages, plus About and Services pages.
Admin dashboard: The Django admin manages users, events and uploaded Excel files.

 🛠️ Technology Stack

| Component             | Technologies          |
| --------------------- | --------------------- |
| Programming Language  | Python                |
| Backend Framework     | Django                |
| Frontend Technologies | HTML, CSS, JavaScript |
| Database              | SQLite                |
| Data Analysis         | Pandas, NumPy         |
| Machine Learning      | Scikit-learn          |

 📂 Project Structure

```text
miniproject/
│
├── authentication/        # Main app: user model, forms, views, templates, static files
├── navigation/            # Serves the landing page
├── placement_site/        # Project settings and root URL configuration
├── website/               # Supporting copy of the model test script, dataset and manage.py
├── media/
│   └── excel_files/       # Excel files uploaded by the admin
├── model_campus_placemen  # Trained Logistic Regression model (Joblib)
├── student_data.csv       # Training dataset
├── manage.py
├── requirements.txt
└── README.md
```

 ⚙️ Installation and Execution

 📋 Prerequisites

* Python 3.x
* pip
* Git

📥 Clone the Repository

```bash
git clone https://github.com/Blessy-Anna-Benny/miniproject.git
```

 📁 Navigate to the Project Directory

```bash
cd miniproject
```

🔧 Create a Virtual Environment

```bash
python -m venv venv
```

 ▶️ Activate the Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

 🗄️ Apply Database Migrations

```bash
python manage.py migrate
```

 🚀 Run the Development Server

```bash
python manage.py runserver
```

🌐 Access the Application

Open your browser and navigate to:

```text
http://127.0.0.1:8000/
```

🎯 Technical Contributions and Learning Outcomes

* Designed a custom Django user model with AbstractUser to store student academic records.
* Built registration, login and password-change flows using Django forms and authentication.
* Trained a scikit-learn Logistic Regression model and integrated it into a Django view with Joblib for real-time predictions.
* Implemented Excel upload through the Django admin and rendered the data as HTML tables with Pandas.
 * Organised the project into modular Django apps with separate templates, static files and URL configuration.




