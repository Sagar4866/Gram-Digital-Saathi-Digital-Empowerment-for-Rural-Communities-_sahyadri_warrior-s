🌱 Gram Digital Saathi
Digital Empowerment for Rural Communities (AVS318 Project)

A Progressive Web App (PWA) + Admin Dashboard designed to empower rural communities with digital literacy, offline-first learning, QR-driven content access, and local analytics tracking.

📌 Project Summary

Rural communities often struggle with low digital literacy, limited internet connectivity, and lack of access to essential digital services like government schemes, online payments, healthcare portals, and digital learning.

Gram Digital Saathi solves this problem through a lightweight, offline-capable digital learning platform designed specifically for low-end devices, low bandwidth areas, and first-time digital users.

The system works fully offline after first load, includes local data storage, and enables trainers/community volunteers to teach using QR codes, short videos, and interactive lessons.

🌟 Key Features
1️⃣ Digital Literacy Lessons (Marathi)

Short, simplified micro-lessons

UPI, Aadhaar, online govt services

Built-in Text-to-Speech (TTS) in Marathi

QR-linked lessons for instant access

2️⃣ Offline-First PWA

Works without internet after first visit

Cache-first Service Worker

Static content (JSON-based lessons, forms, videos)

3️⃣ Rural-Friendly Visual Interface

Large icons, simple UI

No login required for learners

Supports mobile browsers & KaiOS-style phones

4️⃣ QR Scan & QR Generate

Each lesson has a unique QR

Scan → open lesson instantly

Google Chart API for QR generation

5️⃣ Forms & Helpdesk (Local Storage)

Govt scheme enquiry forms

Health appointment form

Saves data locally for demo

Admin can view submissions

6️⃣ Local Event Analytics (Offline)

Tracks: lesson opens, TTS usage, form submissions, QR scans

Stored in localStorage

Admin dashboard shows charts using Chart.js

🏗️ Tech Stack
Frontend (Primary for Demo)

HTML, CSS, JavaScript

Chart.js (Analytics)

html5-qrcode (Camera QR scanner)

PWA (Manifest + Service Worker)

LocalStorage for offline data

TTS (Marathi) via Web Speech API

Backend (Optional for Full Production)

Django REST API

Users, Courses, Schemes

Progress tracking

PostgreSQL (Production)

SQLite (Local Dev)

Analytics (Optional Integration)

Metabase (self-hosted)

Plausible (lightweight)

OpenSearch Dashboard

🚀 How to Run the Demo
cd gram-digital-frontend-demo/public
python3 -m http.server 8000


Open:
👉 http://localhost:8000/index.html

Works offline after loading once.

🧱 Folder Structure (Frontend Demo)
public/
│── index.html
│── lesson.html
│── admin.html
│── app.js
│── admin.js
│── offline-storage.js
│── qr-helper.js
│── lessons.json
│── forms.json
│── styles.css
│── sw.js
└── assets/
    ├── videos/
    └── icons/

🧩 Why This Project? (AVS318 Justification)

Addresses the digital divide in rural regions

Provides affordable, low-bandwidth learning tools

Works offline, solving rural internet challenges

Provides analytics to track progress

Helps learners access government services confidently

QR-based microlearning supports on-ground trainers
