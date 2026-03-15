# GfG Campus Club Website Challenge Portal

A full-stack web platform built for the **GeeksforGeeks Campus Club – Rajalakshmi Institute of Technology Website Building Challenge 2026**.

This portal provides a centralized platform for managing campus club activities, events, and learning resources. It includes a public-facing website for participants and a restricted administrative workspace for club coordinators to manage events, registrations, and resources efficiently.

---

## Key Features

* Public website for browsing club content without mandatory login
* Event listings with individual event registration pages
* Learning resources with categories, difficulty level, duration, and external links
* Leaderboard to showcase participant performance
* FAQ, Contact, and About pages for user support
* Dedicated judge navigation guide for evaluation

---

## Advanced Features

* **Dynamic Event Registration System**
  Each event can define its own custom registration form fields tailored to the event requirements.

* **Configurable Registration Controls**
  Events support registration limits and can be toggled between open or closed states.

* **Optional Participant Email Requirement**
  Events can require participants to provide an email address during registration if needed.

* **Participant List Generation**
  Admins can generate participant lists from submitted registrations with customizable field selection.

* **Export Support for Registrations**
  Participant data can be exported in **CSV** or **PDF** formats for reporting and management.

* **Role-Based Admin Control**
  Admins can promote users to **coordinator roles** or revoke coordinator access for controlled management.

* **Hidden Admin Login Entry**
  The administrative dashboard is protected behind a hidden login in the college logo(RIT) /route to reduce unauthorized discovery.

* **First-Admin Bootstrap Setup**
  A bootstrap mechanism allows the first administrator account to initialize the system securely.

* **Secure Authentication System**
  Session-based authentication with **password hashing** ensures secure login handling.

* **OTP-Based Password Reset**
  Users can reset passwords using a **One-Time Password (OTP)** verification flow.

* **Judge Access Guide Page**
  A dedicated guide page is included to help judges quickly navigate and evaluate the platform features.

---

## Technology Stack

### Backend

* Python
* Flask
* SQLite Database

### Frontend

* HTML Templates
* CSS
* JavaScript

### Tools

* GitHub for version control
* VS Code for development

---

## Run Locally

Create a virtual environment and install dependencies.

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Open in browser:

http://127.0.0.1:5000

---

## Deployment

This project can be deployed on platforms that support Flask applications such as:

* Render
* Railway
* PythonAnywhere
* VPS hosting

The repository includes a **Procfile** for platforms that automatically detect Gunicorn.

### Production Start (Windows)

```powershell
pip install waitress
waitress-serve --listen=0.0.0.0:8080 app:app
```

### Production Start (Linux)

```bash
pip install -r requirements.txt
gunicorn app:app
```

---

## Judge Access Guide

A special **judge navigation page** is included in the platform in the 3 dot button in the navigation/top bar to help evaluators quickly explore and test the system features.

The guide explains:

* how to access different sections of the website
* how to test event registrations
* how to access administrative functionality

---

## Contributors

* **TEAM BULDERS**
