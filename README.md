# Employee REST API Testing (Postman + Newman)

## 📌 Project Overview

This project demonstrates API testing for an Employee Management System using Postman.
It includes 20+ test cases covering both positive and negative scenarios.

The testing workflow includes:

* Authentication (Login API)
* Employee creation
* Data validation
* Update operations
* Deletion operations
* Query parameter validation

---

## 🛠 Tools & Technologies

* Postman
* Newman
* Node.js
* GitHub

---

## 🌐 API Documentation

Base API and endpoints are available here:
https://documenter.getpostman.com/view/25113210/2sB3BLhSC1

---

## ⚙️ Environment Setup

* Environment Name: **TestEnv**
* All requests and test cases are executed within this environment.

---

## ✅ Test Scenarios Covered

### 1. Login API

* Valid login (positive)
* Invalid credentials (negative)
* Missing fields validation
* Unauthorized access handling

### 2. Create Employee

* Create 5 employees with random data:

  * First Name
  * Last Name
  * Email
  * Phone
  * Department
  * Position
  * Salary
* Validate successful creation (status code, response body)

### 3. Get Employee Info

* Retrieve created employees
* Validate:

  * Employee existence
  * Correct department mapping

### 4. Update Employee Info

* Update:

  * Mobile number
  * Position
* Validate updated response

### 5. Delete Employee

* Delete 1 employee
* Validate:

  * Successful deletion response
  * Employee no longer exists

### 6. Get Employees with Query Params

* Fetch all employees
* Validate total employee count

---

## 🧪 Test Cases

* Total Test Cases: **20+**
* Includes:

  * Positive scenarios
  * Negative scenarios
  * Edge cases

---

## 📦 Postman Collection

👉 Add your exported collection link here
Example:

```
[Postman Collection](your-link-here)
```

---

## 📊 Newman Report

Run tests using Newman:

```bash
newman run collection.json -e environment.json -r cli,html
```

---

## 📸 Newman Report Screenshots

(Add screenshots here)

---

## 📄 Postman Documentation

👉 Add your published documentation link here

---

## 📁 Project Structure

```
├── collection.json
├── environment.json
├── newman-report.html
├── screenshots/
└── README.md
```

---

## 🚀 How to Run

1. Clone the repository
2. Install Newman:

```bash
npm install -g newman
```

3. Run the collection:

```bash
newman run collection.json -e environment.json
```

---

## 👤 Author

Rezwanul Islam Rimel – SQA Engineer

---

## 📌 Notes

* All test data is randomly generated
* Tests include assertions for status codes and response validation
* Designed for learning and demonstration purposes
