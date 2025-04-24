# 🏫 School Management API

A Node.js REST API built using **Express.js** and **MySQL** that allows users to:

- 📌 Add a new school with geolocation (latitude, longitude)
- 📍 List all schools sorted by proximity to a given user location

Hosted on **Render**, connected to a **MySQL** database hosted on [FreeSQLDatabase](https://www.freesqldatabase.com/).

---


## 🔧 Technologies Used

- Node.js
- Express.js
- MySQL
- mysql2
- dotenv
- Postman (for API testing)

---

## 🌐 API Endpoints

### ➕ Add School

**POST** `/api/addSchool`

**Request Body:**

{
  "name": "Green Valley High",
  "address": "123 Hill Road",
  "latitude": 22.5726,
  "longitude": 88.3639
}

Response:

{
  "message": "School added successfully"
}


###📍 List Schools by Proximity
** GET ** `/api/listSchools?latitude=22.5726&longitude=88.3639`

Response:


  {
    "id": 1,
    "name": "Green Valley High",
    "distance_km": 1.23
  },
  ...


