# 🎓 Scholarship Auto-Filer for Indian ST Students

**Scholarship Auto-Filer** is an automated web application designed for Indian Scheduled Tribe (ST) students pursuing higher education. It streamlines central fellowship & scholarship applications (**NFST**, **NOS**, and **Post-Matric Scholarship**) using Gemini 2.0 Flash AI vision document extraction and deterministic backend eligibility rule matching.

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-v22+-green.svg)
![React](https://img.shields.io/badge/React-18-blue.svg)
![Gemini AI](https://img.shields.io/badge/AI-Gemini%202.0%20Flash-orange.svg)

---

## 🌟 Key Features

- 📑 **AI Vision Document Extraction**: Upload Caste Certificates, Marksheets, Income Certificates, and Bank Passbooks — Gemini AI extracts fields automatically.
- 🎯 **Deterministic Scheme Eligibility Rules**: Calculates scheme qualifications against official Ministry rules (income caps, course levels, min marks %).
- ✍️ **Auto-Filled Editable Application**: Automatically populates submission forms with extracted data while allowing applicant edits.
- 📊 **Ministry Reviewer Admin Workspace**: Review applications, filter by scheme/status, view aggregate stats, and approve/reject applications with review notes.
- 🔒 **Privacy First & Secure**: Role-based access control with JWT authentication ensuring applicant PII security.

---

## 🏗️ Technology Stack

- **Frontend**: React 18, Vite, React Router DOM v6, Lucide Icons.
- **Backend**: Express (Node.js v22), native SQLite (`node:sqlite`), JWT Auth, `bcryptjs`.
- **AI Integration**: `@google/generative-ai` (Gemini 2.0 Flash Vision).
- **Design System**: Light-mode government portal UI (Navy Blue `#0B2545`, Slate `#1E293B`, Saffron Amber `#D97706`, Emerald `#059669`).

---

## 🚀 Quick Start Guide

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/scholarship-auto-filer.git
cd scholarship-auto-filer
```

### 2. Install Dependencies
```bash
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

### 3. Configure Environment Variables
Create a `.env` file in the `backend/` directory:
```env
PORT=5000
JWT_SECRET=scholarship-autofiler-super-secret-key-2026
GEMINI_API_KEY=YOUR_GEMINI_API_KEY_HERE
```

### 4. Build and Run
```bash
# Build frontend static bundle
cd frontend
npm run build

# Start backend server
cd ../backend
npm start
```
Open your browser at **`http://localhost:5000`**.

---

## 🔑 Demo Login Accounts

| Role | Email | Password |
| :--- | :--- | :--- |
| **ST Student / Applicant** | `rahul.st@example.com` | `student123` |
| **Ministry Admin / Reviewer** | `admin@tribal.gov.in` | `admin123` |

---

## 📄 License
MIT License. Created for Ministry of Tribal Affairs ST scholarship application automation.
