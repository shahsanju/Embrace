# 🎓 Embrace – Alumni Connect Platform

A full-stack alumni networking platform built for colleges, featuring a web portal, real-time chat, and a mobile app.

---

## 📌 About the Project

Embrace is a platform that connects college students with alumni. It allows alumni to register, share job opportunities, post in forums, schedule meetings, and chat in real time. Admins can manage users, events, gallery, courses, and site settings through a dedicated dashboard.

---

## 🏗️ Project Structure

```
Embrace/
├── college/          # PHP Web Application (Frontend + Backend)
│   ├── admin/        # Admin dashboard (manage users, events, jobs, forums)
│   ├── database/     # MySQL database schema
│   └── ...           # Alumni-facing pages (home, login, signup, forum, etc.)
├── chat_app/         # Real-time Chat Server (Node.js + Socket.IO)
└── embrance/         # Mobile App (Flutter)
```

---

## ✨ Features

- Alumni registration, login, and profile management
- Admin dashboard to manage alumni, events, jobs, courses, and gallery
- Discussion forums and comment system
- Job board for career opportunities
- Real-time one-on-one chat between users
- Meeting scheduling between alumni and students
- Mobile app (Flutter) for on-the-go access

---

## 🛠️ Technologies Used

| Layer | Technology |
|-------|-----------|
| Web Frontend | HTML, CSS, JavaScript, PHP |
| Backend | PHP, MySQL |
| Real-time Chat | Node.js, Express, Socket.IO |
| Mobile App | Flutter (Dart) |
| Database | MySQL |

---

## ⚙️ How to Run

### Prerequisites
- PHP and a local server like **XAMPP** or **MAMP**
- **MySQL** database
- **Node.js** (v14 or above)
- **Flutter SDK** (for mobile app)

---

### 1️⃣ Set Up the Database

1. Open **phpMyAdmin** (comes with XAMPP/MAMP)
2. Create a new database called `alumni_db`
3. Import the file `college/database/alumni_db.sql` into it

---

### 2️⃣ Run the Web App (PHP)

1. Copy the `college/` folder into your XAMPP/MAMP `htdocs` directory
2. Open `college/admin/db_connect.php` and make sure the credentials match your setup:
   ```php
   $conn = new mysqli('localhost', 'root', '', 'alumni_db');
   ```
3. Start Apache and MySQL from XAMPP/MAMP
4. Open your browser and go to:
   ```
   http://localhost/college/
   ```

---

### 3️⃣ Run the Chat Server (Node.js)

Open a terminal and run:

```bash
cd chat_app
npm install
node index.js
```

The chat server will start on **port 8080**.

---

### 4️⃣ Run the Mobile App (Flutter)

```bash
cd embrance
flutter pub get
flutter run
```

Make sure your device/emulator is connected before running.

---

## 👥 Authors

- **Sanjana Shah** — [@shahsanju](https://github.com/shahsanju)
