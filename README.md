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
  <img width="1894" height="903" alt="Screenshot_2025-09-19_205217 1" src="https://github.com/user-attachments/assets/b6d8e7be-be56-4023-8aaa-270f1ebb90ca" />
  <br>
  <em>Admin dashboard displaying doctors and appointments</em>
  <br><br>
  <img width="1896" height="876" alt="Screenshot_2025-09-19_205323 1" src="https://github.com/user-attachments/assets/4683bbac-d90a-44b0-9109-6ef547beb300" />
  <br><br>
  <img width="1882" height="887" alt="Screenshot_2025-09-19_205257 1" src="https://github.com/user-attachments/assets/60c76859-c9fe-49c9-9282-77bc7f94368f" />
</p>

---
⭐ **If you like this project, give it a star on GitHub!**
