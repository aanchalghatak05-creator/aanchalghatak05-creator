# Data Journalism Portfolio — Full Stack Web Application

**Live Demo:** [https://cmt-120-cw-2-git-cmt120-cw.apps.containers.cs.cf.ac.uk](https://cmt-120-cw-2-git-cmt120-cw.apps.containers.cs.cf.ac.uk)

A full-stack web application built to showcase data journalism work, including written articles, data-driven stories, and multimedia content. Developed as part of CMT120 – Fundamentals of Programming at Cardiff University and deployed to production on OpenShift.

---

## 🚀 Live Deployment

| Detail | Info |
|---|---|
| Platform | Red Hat OpenShift (Cardiff University) |
| URL | https://cmt-120-cw-2-git-cmt120-cw.apps.containers.cs.cf.ac.uk |
| Server | Gunicorn (WSGI) |
| Container | Docker |

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python 3, Flask |
| Database | SQLite3 |
| Frontend | HTML5, CSS3, JavaScript (ES6) |
| Async | AJAX (dynamic content filtering without page reload) |
| Auth | Session-based authentication |
| Deployment | Gunicorn · Docker · OpenShift (Red Hat) |

---

## ✨ Features

- **Content Management** — Admin interface to create, edit, and remove articles without modifying source code
- **Searchable Archive** — Written content filterable by year and category using AJAX
- **Multimedia Support** — YouTube integration with auto-generated thumbnails via pattern-matching logic
- **Contact Form** — Asynchronous submissions with real-time feedback, persisted to database
- **Secure Admin Routes** — Session-based authentication protecting all administrative actions
- **Production Deployment** — Containerised with Docker, deployed on OpenShift, served via Gunicorn

---

## 📁 Project Structure

```
├── main.py              # Application logic, routing, and database handling
├── templates/           # Jinja2 templates for page rendering
├── static/
│   ├── css/style.css    # Editorial styling and responsive layout
│   └── js/main.js       # Client-side logic and AJAX functionality
├── content.db           # SQLite database
├── Dockerfile           # Container configuration
├── Procfile             # Gunicorn process declaration
└── requirements.txt     # Python dependencies
```

---

## 🏃 Running Locally

```bash
git clone https://github.com/aanchalghatak05-creator/cmt120-cw2.git
cd cmt120-cw2
pip install -r requirements.txt
python main.py
```

Or with Docker:

```bash
docker build -t journalism-portfolio .
docker run -p 5000:5000 journalism-portfolio
```

---

## 👤 About

Built by **Aanchal Ghatak** — Data Journalist & MSc Computational and Data Journalism student at Cardiff University.

[LinkedIn](https://linkedin.com/in/aanchal-ghatak-496b3561) · [GitHub](https://github.com/aanchalghatak05-creator)
