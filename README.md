# 🎓 Embrace – Supporting Female Students in ECS

> Master's Project — California State University, Sacramento (Spring 2024)  
> Approved by Dr. Anna Baynes (Committee Chair) & Dr. Ahmed Salim (Second Reader)

---

## 📌 About the Project

**Embrace** is a full-stack platform designed to empower female undergraduate students majoring in Engineering and Computer Science (ECS) at Sac State. Inspired by the gender gap in ECS fields — where only 8.4% of Sac State graduates are female ECS majors — this project provides a single platform with all the support a female student might need throughout her academic journey.

The platform consists of three components working together:
- A **Flutter iOS mobile app** for students
- A **PHP web admin panel** for university administrators
- A **Node.js real-time chat server** using Socket.IO

---

## ✨ Features

### 📱 Mobile App (for students)
- **Job Discovery** — Browse job postings with salary info and requirements
- **Roadmap** — Course recommendations tailored to specific career goals
- **Alumni Connect** — Network and chat with alumni
- **Senior Connect** — Connect with senior students for mentorship; schedule meetings
- **Scholarship Search** — Filter and explore available financial aid
- **News Feed** — Real-time IT industry news and articles
- **Event Notifications** — University event reminders pushed from admin
- **Role-Based Access** — Different views for current students, seniors, alumni, and male users

### 🖥️ Admin Panel (for university staff)
- Manage users (verify, view, delete accounts)
- Post and manage job listings, events, scholarships, and courses
- Gallery management
- View alumni and student data

### 💬 Chat Server
- Real-time one-on-one messaging using Socket.IO
- Meeting scheduling between students and seniors/alumni

---

## 🏗️ Project Structure

```
Embrace/
├── college/          # PHP Web Admin Panel
│   ├── admin/        # Admin dashboard (users, jobs, events, scholarships, courses)
│   ├── database/     # MySQL schema (alumni_db.sql)
│   └── ...           # Student-facing pages
├── chat_app/         # Real-time Chat Server (Node.js + Socket.IO)
└── embrance/         # iOS Mobile App (Flutter/Dart)
```

---

## 🛠️ Technologies Used

| Component | Technology |
|-----------|-----------|
| Mobile App | Flutter (Dart), Cupertino & Material widgets |
| Admin Web Panel | PHP, HTML, CSS, JavaScript, AJAX |
| Real-time Chat | Node.js, Express, Socket.IO |
| Database | MySQL |
| Local Storage (App) | SQLite |
| Data Format | JSON / REST API |

---

## ⚙️ How to Run

### Prerequisites
- **XAMPP** or **MAMP** (for PHP + MySQL)
- **Node.js** v14 or above
- **Flutter SDK** (for mobile app)

---

### 1️⃣ Set Up the Database
1. Open **phpMyAdmin**
2. Create a new database named `alumni_db`
3. Import `college/database/alumni_db.sql`

---

### 2️⃣ Run the Admin Web Panel (PHP)
1. Copy the `college/` folder into your XAMPP/MAMP `htdocs` folder
2. Start **Apache** and **MySQL** from XAMPP/MAMP
3. Open your browser and visit:
```
http://localhost/college/
```

---

### 3️⃣ Run the Chat Server (Node.js)
```bash
cd chat_app
npm install
node index.js
```
Chat server runs on **port 8080**.

---

### 4️⃣ Run the Mobile App (Flutter)
```bash
cd embrance
flutter pub get
flutter run
```
Make sure an iOS simulator or device is connected.

---

## 👩‍💻 Author

**Sanjana Shah** — [@shahsanju](https://github.com/shahsanju)  
Master of Science in Computer Science  
California State University, Sacramento — Spring 2024
