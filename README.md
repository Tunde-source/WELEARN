# WELEARN
A digital learning platform 
# 🎯 WELEARN — Digital Skills Learning Platform

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![SDG 4](https://img.shields.io/badge/SDG-4%20Quality%20Education-green)
![Status](https://img.shields.io/badge/Status-In%20Development-orange)
![Platform](https://img.shields.io/badge/Platform-Web-lightgrey)

> **A digital skills-learning platform bridging formal education and industry-relevant employability for youth in Sierra Leone.**

-----

## 📌 Overview

WELEARN equips youth and young professionals with practical, career-focused skills across nine domains, helping close the gap between formal education and labour market demand.

|Fact               |Detail                                                     |
|-------------------|-----------------------------------------------------------|
|**University**     |Limkokwing University of Creative Technology — Sierra Leone|
|**SDG Alignment**  |SDG 4 — Quality Education                                  |
|**License**        |MIT Open Source                                            |
|**Academic Period**|March 2026 – July 2026                                     |

**Mission:** To provide accessible, affordable, and industry-relevant digital skills training that prepares young people for employment and entrepreneurship opportunities.

**Vision:** To become Sierra Leone’s leading digital learning platform for developing job-ready skills and fostering lifelong learning.

-----

## 🚀 Features

- 🔑 **Social sign-up** — register instantly with Google or Facebook
- 📚 **9 skill categories** — Programming, Design, Arts & Crafts, Accounting, Economics, Marketing, Database Management, Digital Imaging, Data Analysis
- 🧩 **Structured subtopics** — e.g. Programming → HTML/CSS, JavaScript, Programming Logic
- 📈 **Progress tracking** — visual completion indicators per course
- 🏅 **Certificates** — auto-generated PDF certificates on course completion
- 👩‍🏫 **Instructor tools** — course creation, content upload, enrolment monitoring
- 🛡️ **Admin panel** — user management, instructor approval, analytics

-----

## 🏗️ System Architecture

```
CLIENT LAYER
├── React.js Web App (Progressive Web App — desktop & mobile)
├── Instructor Portal
└── Admin Panel

CDN / LOAD BALANCER
├── AWS CloudFront (CDN — static assets)
├── AWS Elastic Load Balancer (API traffic)
└── Auth Service (OAuth — Google/Facebook sign-up)

APPLICATION LAYER
├── Node.js + Express REST API (business logic, JWT auth)
├── Certificate Service (PDF generation)
└── Notification Service

DATA LAYER
├── PostgreSQL — AWS RDS (users, courses, progress, certificates)
├── AWS S3 (course content: videos, slides, PDFs)
└── Redis — ElastiCache (session cache)
```

-----

## 🛠️ Technology Stack

|Layer   |Technology                   |
|--------|-----------------------------|
|Web     |React.js 18 + Vite           |
|Backend |Node.js 20 + Express 4       |
|Database|PostgreSQL 15 (AWS RDS)      |
|Cache   |Redis (AWS ElastiCache)      |
|Storage |AWS S3 + CloudFront          |
|Auth    |JWT + OAuth 2.0 (Passport.js)|
|CI/CD   |GitHub Actions               |
|Testing |Jest + Supertest             |

-----

## 📁 Repository Structure

```
welearn-digital-public-good/
├── /client          → React.js web app
├── /server          → Node.js + Express API
├── /database        → SQL schema & migrations
├── /docs             → Report, UML diagrams, architecture
├── /prototype        → Figma exports (10 screens)
├── /tests             → Unit & integration tests
├── /.github/         → GitHub Actions CI/CD workflows
├── README.md
└── LICENSE
```

-----

## ⚙️ Getting Started

```bash
# Clone the repository
git clone https://github.com/[your-username]/welearn-digital-public-good.git
cd welearn-digital-public-good

# Install backend dependencies
cd server && npm install

# Install frontend dependencies
cd ../client && npm install

# Set up environment variables
cp .env.example .env

# Run database migrations
cd ../server && npm run migrate

# Start development servers
npm run dev                    # starts API on port 3001
cd ../client && npm run dev    # starts web app on port 3000
```

-----

## 🧪 Running Tests

```bash
npm run test               # Unit tests
npm run test:integration   # Integration tests
npm run test:coverage      # Coverage report
```

-----

## 🤝 Contributing

1. Fork the repository
1. Create a feature branch: `git checkout -b feature/your-feature-name`
1. Commit using Conventional Commits: `git commit -m "feat: add certificate generation"`
1. Push and open a Pull Request — at least 1 reviewer approval required before merge

-----

## 📄 License

This project is licensed under the **MIT License** — see the <LICENSE> file for details.

-----

## 🌐 SDG 4 Impact

|SDG 4 Target                                     |WELEARN Response                                     |
|-------------------------------------------------|-----------------------------------------------------|
|4.3 — Affordable technical & vocational education|Free/low-cost skills courses, open to all backgrounds|
|4.4 — Relevant skills for employment             |Job-market-aligned curriculum across 9 domains       |
|4.5 — Eliminate access disparities               |Frictionless social sign-up, mobile-responsive design|
|4.7 — Knowledge for sustainable development      |Practical skills tied to local economic opportunity  |

-----

## 📬 Contact

**Faculty of Information and Communication Technology**
Limkokwing University of Creative Technology — Sierra Leone
Academic Period: March 2026 – July 2026

-----

*WELEARN is a Digital Public Good committed to bridging education and employability for Sierra Leone’s youth.*
