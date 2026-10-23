# SchoolFlow - School Management System (Offline Edition)

## 📌 Project Overview
SchoolFlow ek modern aur Offline Desktop Software hai jo schools ke rozmarra ke kaamon ko digitally manage karne ke liye design kiya gaya hai. Iska maqsad school ke manual record (registers) ko khatam karke ek aisa secure system dena hai jo bina internet ke bhi kaam kare. 

## 🎯 Purpose 
Aaj kal online systems internet par depend karte hain. SchoolFlow ka maqsad hai ke Principal, Teachers aur Admin bina internet ke apna poora record manage kar sakein. Data local computer par (SQLite mein) mehfooz hoga, jisse privacy aur speed dono behtar hongi.

## 🛠️ Tech Stack (Technologies Used)
- **Frontend:** Next.js (React), TypeScript, Bootstrap/Tailwind CSS
- **Backend:** NestJS (Node.js), TypeScript
- **Database:** SQLite (Offline), Prisma ORM
- **Desktop App:** Electron.js
- **Security:** JWT, Bcrypt

## 📂 Project Structure
Humara project **Monorepo** architecture follow karta hai:
- `apps/web`: Frontend (Next.js)
- `apps/api`: Backend (NestJS)
- `apps/desktop`: Electron App
- `packages/`: Shared database (Prisma) aur types
- `docs/`: Project ki requirements aur progress logs

## 👨‍💻 Development Methodology
Hum is project ko **Spec-Driven Development (SDD)** ke through phase-by-phase bana rahe hain.