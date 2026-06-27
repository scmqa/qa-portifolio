# API Testing Project - JSONPlaceholder Users API

## 📌 Overview

This project demonstrates API testing using *Postman* on the JSONPlaceholder fake REST API.

The objective was to validate the /users endpoint by performing CRUD operations and creating automated tests to verify response status codes, response time, headers, and JSON data integrity.

---

## 🛠️ Tools

- Postman
- JSONPlaceholder API
- REST API
- JavaScript (Postman Tests)

---

## 📋 Endpoints Tested

### GET /users
Validated:
- Status Code (200)
- Response Time
- Content-Type
- Total number of users
- Email validation
- Phone validation
- Website validation
- Unique IDs
- IDs greater than zero
- City field
- Zip Code field
- Geo coordinates

### POST /users
Validated:
- Status Code (201)
- Response contains ID
- Returned name
- Returned email

### PUT /users/1
Validated:
- Status Code (200)
- Updated name
- User ID
- Email

### DELETE /users/1
Validated:
- Status Code (200)
- Empty response body

---

## 📊 Test Summary

| Method | Status |
|---------|--------|
| GET | ✅ Passed |
| POST | ✅ Passed |
| PUT | ✅ Passed |
| DELETE | ✅ Passed |

---

## 📂 Project Structure


API-Testing-Project/
│
├── README.md
├── API_Testing_Report_JSONPlaceholder.pdf
└── Evidence/
    ├── GET-users-tests.png
    ├── POST-users-tests.png
    ├── PUT-users-tests.png
    └── DELETE-users-tests.png


---

## 🎯 Skills Demonstrated

- API Testing
- REST API
- CRUD Operations
- Automated Testing with Postman
- JSON Validation
- Response Validation
- Test Documentation
- QA Best Practices

---

## 👩‍💻 Author

*Silmara Costa*

QA Automation | API Testing | Software Testing | Postman
