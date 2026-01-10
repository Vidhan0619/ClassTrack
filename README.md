📚 ClassTrack – Smart Classroom & Lab Availability System

ClassTrack is a web-based smart campus solution that helps students and faculty check real-time availability of classrooms and laboratories, manage schedules, view notices, and interact through a campus community — all powered by Firebase Authentication and Firestore.


---

🚀 Features

👨‍🎓 Student Features (Read-Only)

View real-time classroom & lab availability

Search rooms instantly

View weekly utilization (analytics)

Access Notice Board (club events & announcements)

Participate in Community section (student–senior interaction)

Mobile-responsive UI


👩‍🏫 Faculty Features (Admin)

Secure Admin Panel

Read & Write access to Firestore

Manage classroom & lab schedules

Book extra classes/labs

Automatic expiry of extra bookings

View usage analytics (charts)

View room-wise timetable



---

🏗️ Tech Stack

Technology	Usage

HTML5	Structure
CSS3	Responsive UI & Theme
JavaScript (ES6)	Logic
Firebase Authentication	Google Login (College Email Only)
Firebase Firestore	Real-time Database
Chart.js	Analytics & Utilization Graphs



---

🔐 Authentication Rules

Only college email IDs can log in

Students → Read-only access

Faculty (Admins) → Read & Write access



---

📂 Project Structure

ClassTrack/
│
├── login.html
├── dashboard.html
├── class.html
├── lab.html
├── admin.html
├── notice.html
├── community.html
│
├── common.css
├── dashboard.css
├── admin.css
├── style.css
│
├── firebase-config.js (optional)
└── README.md


---

🔥 Firebase Setup

1. Create a Firebase project


2. Enable:

Authentication → Google Provider

Cloud Firestore



3. Add your Firebase config to all JS files


4. Firestore structure example:



Classroom (collection)
 ├── A221 (document)
 │    ├── type: "Classroom"
 │    ├── schedule: [ { day, start, end } ]
 │
 ├── LAB1 (document)
 │    ├── type: "Lab"
 │    ├── software: ["Python", "MATLAB"]


---

📊 Workflow Overview

1. User opens website


2. Firebase Authentication checks role


3. Student

Reads data from Firestore



4. Faculty

Reads & writes schedules



5. Firestore updates reflect in real-time UI




---

📱 Responsive Design

Optimized for mobile, tablet, and desktop

Single-column cards on phones

Collapsible hamburger menu

Clean & accessible UI



---

👥 Team Collaboration (Group Project)

GitHub repository shared with teammates

Faculty & student roles clearly defined

Contributions managed using GitHub collaborators



---

🛠️ Future Enhancements

Push notifications

Role-based admin approval

Room booking conflict prevention

Attendance integration

AI-based usage optimization



---

📜 License

This project is created for educational purposes.
You are free to modify and enhance it.


---

🙌 Acknowledgements

Firebase Team

Chart.js

Font Awesome

OpenAI (for development assistance)

