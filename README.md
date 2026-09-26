# OM MISHRA PRODUCTIONS

# 🚀 HackTrack — Hackathon Management System

> **Turning hackathon chaos into organized innovation.**

HackTrack is a modern, full-stack hackathon management platform designed to streamline the complete hackathon lifecycle — from participant registration and team management to QR-based check-ins, judging, certificates, food distribution, and live leaderboards.

The platform provides dedicated dashboards and role-based access for **Participants, Judges, Admins, and Super Admins**, making hackathon operations easier to manage from a centralized system.

---

## ✨ Key Features

### 👨‍💻 Participant Portal

- User registration and authentication
- Team management
- QR-based event check-in
- Food distribution QR
- Problem statement access
- Project information
- Certificate generation/download
- Event photos
- Participant dashboard

### ⚖️ Judge Portal

- View assigned teams
- Evaluate projects
- Submit marks
- Edit evaluations
- Provide feedback
- View previous evaluations

### 🛠️ Admin Portal

- Participant management
- Team management
- Bulk user import
- Check-in management
- QR verification
- Food distribution management
- Event dashboard

### 👑 Super Admin Portal

- Complete system management
- User management
- Team management
- Judge assignment
- Problem statement assignment
- Participant management
- Live leaderboard
- Event administration

### 🔐 Security

- JWT-based authentication
- Role-Based Access Control (RBAC)
- Protected routes
- Role-specific dashboards
- Permission-based navigation

---

## 🏗️ System Architecture

```text
                         ┌──────────────────┐
                         │      Users       │
                         └────────┬─────────┘
                                  │
                                  ▼
                         ┌──────────────────┐
                         │  React Frontend  │
                         │    Vite + React  │
                         └────────┬─────────┘
                                  │
                                  │ REST API
                                  ▼
                         ┌──────────────────┐
                         │  Express Server  │
                         │    Node.js       │
                         └────────┬─────────┘
                                  │
                    ┌─────────────┴─────────────┐
                    ▼                           ▼
             ┌──────────────┐           ┌──────────────┐
             │   MongoDB    │           │    Redis     │
             │   Database   │           │    Cache     │
             └──────────────┘           └──────────────┘
