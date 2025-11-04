# 🏥 Hospital Management System

A full-stack web application that simplifies hospital operations — from patient registration and doctor management to appointment scheduling and medical record tracking.
Built using **Node.js**, **Express.js**, **MongoDB**, and **Mongoose**, it provides a smooth and efficient interface for hospital administration.

---

## 🧠 Overview

The **Hospital Management System** streamlines daily hospital tasks by digitizing essential operations.
It allows admins, doctors, and patients to manage:

* 👩‍⚕️ Doctor profiles
* 🧍 Patient registration and records
* 📅 Appointment scheduling
* 🧾 Medical reports and records

This project follows a **RESTful architecture**, using **MongoDB** as the backend database and **Express.js** as the API framework.

---

## 🛠️ Tech Stack

| Layer                     | Technology                 |
| ------------------------- | -------------------------- |
| **Frontend**              | HTML5, CSS3, JavaScript    |
| **Backend**               | Node.js, Express.js        |
| **Database**              | MongoDB (via Mongoose)     |
| **Environment Variables** | dotenv                     |
| **Other Tools**           | nodemon, cors, body-parser |

---

## ✨ Features

✅ Admin can manage doctors, patients, and appointments
✅ Patients can register and view their records
✅ Doctors can access and update patient reports
✅ MongoDB database integration for data storage
✅ RESTful API structure for easy scalability
✅ Secure configuration using `.env` file

---

## 📂 Folder Structure

```
hospital-management-system/
│
├── backend/
│   ├── server.js             # Main server file
│   ├── package.json          # Dependencies and scripts
│   ├── models/               # Database models (Doctor, Patient, Appointment)
│   ├── seed.js               # Data seeding for testing
│   ├── .env                  # Environment variables (MongoDB URI, Port)
│   └── node_modules/         # Installed dependencies
│
└── README.md                 # Project documentation
```

---

## ⚙️ Installation & Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/hospital-management-system.git
   ```

2. **Navigate to Backend Folder:**

   ```bash
   cd hospital-management-system/backend
   ```

3. **Install Dependencies:**

   ```bash
   npm install
   ```

4. **Set Up Environment File (.env):**
   Create a `.env` file inside `backend/` and add:

   ```
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   ```

5. **Run the Server:**

   ```bash
   npm start
   ```

   or (for auto-reload)

   ```bash
   npm run dev
   ```

6. **Access the App:**

   * Open your browser at: `http://localhost:5000`

---

## 🔌 API Overview

| Endpoint            | Method | Description              |
| ------------------- | ------ | ------------------------ |
| `/api/patients`     | GET    | Fetch all patients       |
| `/api/patients`     | POST   | Register a new patient   |
| `/api/doctors`      | GET    | Get list of doctors      |
| `/api/appointments` | POST   | Book a new appointment   |
| `/api/records`      | GET    | Retrieve medical records |

> 🧩 These routes may vary based on your implementation — update this table accordingly.

---

## 💾 Database Schema (Example)

### 🧍 Patient Model

```js
{
  name: String,
  age: Number,
  gender: String,
  contact: String,
  medicalHistory: String
}
```

### 👩‍⚕️ Doctor Model

```js
{
  name: String,
  specialization: String,
  email: String,
  phone: String
}
```

### 📅 Appointment Model

```js
{
  patientId: ObjectId,
  doctorId: ObjectId,
  date: Date,
  status: String
}
```


## 📸 Screenshots

<p align="center">
  <img width="535" height="691" alt="Dashboard" src="https://github.com/user-attachments/assets/example-dashboard.png" />
  <br>
  <em>Admin dashboard displaying doctors and appointments</em>
  <br><br>
  <img width="552" height="719" alt="Patient Page" src="https://github.com/user-attachments/assets/example-patient.png" />
  <br><br>
  <img width="541" height="406" alt="Doctor Management" src="https://github.com/user-attachments/assets/example-doctor.png" />
</p>

---
⭐ **If you like this project, give it a star on GitHub!**
