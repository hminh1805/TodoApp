# 🗓️ Task Scheduler & Automated Notification System

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Vanilla JS](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)

A robust, full-stack task management web application designed and built from scratch as a **Solo Developer**. This system provides a secure, role-based environment for users to schedule events and relies on a background scheduling module to dispatch automated email notifications.

## ✨ Key Features & Architecture

* **Secure Authentication Pipeline:** * Implemented JSON Web Tokens (JWT) stored safely in `HTTP-only` cookies.
  * OTP (One-Time Password) email verification for secure account creation and recovery.
* **Role-Based Access Control (RBAC):**
  * **User:** Can add, update, delete, and view their own scheduled events.
  * **Admin:** Dedicated dashboard to monitor global system metrics and manage user accounts.
* **Automated Background Scheduling:** Utilized `node-schedule` to continuously monitor the MongoDB database and execute timely event reminders via email (`nodemailer`).
* **RESTful API Design:** Clean, modularized routing controllers handling asynchronous client requests, extensively tested with **Postman**.
* **Custom Frontend:** Built with pure Vanilla JS, HTML, and CSS for high performance and full control over DOM manipulation (no heavy frameworks).

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB (Mongoose)
* **Authentication:** JWT, bcrypt
* **Background Jobs & Mail:** Node-Schedule, Nodemailer
* **Frontend:** HTML, CSS, Vanilla JavaScript, AJAX

## 🚀 Installation & Setup

1. **Clone the repository:**
```bash
   git clone [https://github.com/hminh1805/todoapp.git](https://github.com/hminh1805/todoapp.git)
   cd todoapp
```
2. **Install dependencies:**
```bash
npm install
```

3. **Environment Variables:*
Create a .env file in the root directory and configure the following credentials:
```bash
PORT=3000
MONGODB_URI=your_mongodb_connection_string
SECRET_KEY=your_jwt_secret_key
AdminEmail=your_email@gmail.com
AdminEmailPass=your_app_password
AdminRole=admin
AdminName=your_name
AdminPass=your_pass
```

4. **Run the server:**
```bash
node server.js
```
The server will start at http://localhost:3000

