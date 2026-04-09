# <p align="center">🚀 Employee REST API Automation: Postman & Newman</p>

<p align="center">
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
  <img src="https://img.shields.io/badge/Newman-EF5B25?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/API_Testing-Automated-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

---

### 📖 Project Overview
> [!IMPORTANT]
> This project demonstrates a robust **API Testing Framework** for an Employee Management System. It features **20+ Automated Test Cases**, dynamic data generation, and CLI-based execution using Newman for seamless CI/CD integration.

---

## 🛠️ Tech Stack & Integration
* **Core Tool:** `Postman` (Collection & Environment Management)
* **CLI Runner:** `Newman` (Automation & CLI Execution)
* **Scripting:** `JavaScript` (Pre-request & Test Scripts)
* **Reporting:** `Newman-Reporter-HtmlExtra` / `CLI`
* **Documentation:** `Postman Documenter`

---

## 🧪 Testing Coverage & Workflows

#### 🟦 **1. Authentication & Security**
* **Positive:** Valid Login with JWT/Token retrieval.
* **Negative:** Unauthorized access handling & invalid credential validation.

#### 🟧 **2. Dynamic CRUD Operations**
* **Create:** Automated creation of **5 employees** using random data generators.
* **Update:** Selective patching of Mobile Number and Position.
* **Delete:** Resource cleanup validation and 404 verification post-deletion.

#### 🟩 **3. Validation & Assertions**
* **Schema Validation:** Verifying JSON structure and data types.
* **Query Params:** Filtering and validating total record counts via query strings.
* **Status Codes:** Strict adherence to REST standards (200, 201, 400, 401, 404).

---

## 📊 Test Execution Summary

| 📈 Metric | 📋 Details |
| :--- | :--- |
| **Total Test Cases** | <kbd>20+ Scenarios</kbd> |
| **Environment** | `TestEnv` (Dynamic Variables) |
| **Data Handling** | `Pre-request Scripts` for Random Data |
| **Report Format** | `CLI`, `HTML (htmlextra)` |

---

## 🚀 How to Run Locally

#### **1. Prerequisites**
Ensure you have `Node.js` installed. Then, install Newman globally:
```bash
npm install -g newman
npm install -g newman-reporter-htmlextra
```

#### **2. Execution**
Run the following command to execute the collection and generate a premium report:
```bash
newman run collection.json -e environment.json -r cli,htmlextra --reporter-htmlextra-export ./reports/report.html
```

---

## 🐞 Defect Management & Artifacts

> [!NOTE]
> All test data is randomly generated using JavaScript `Math.random()` and `Date.now()` logic within Postman to ensure unique test runs.

* 📂 **[API Documentation](https://documenter.getpostman.com/view/25113210/2sB3BLhSC1):** Full endpoint definitions.
* 📂 **[Postman Collection](./collection.json):** Exported JSON for local import.
* 📂 **[Screenshots](./screenshots):** CLI execution proofs and HTML report dashboard.

---

## 📂 Repository Structure

```text
├── 📂 collections
│   └── employee_api_tests.json
├── 📂 environments
│   └── test_env.json
├── 📂 reports
│   └── automation_dashboard.html
└── 📄 README.md
```

---

## 👤 Author

**Rezwanul Islam**
*SQA Engineer | API Automation Specialist*

<p align="left">
<a href="https://www.linkedin.com/in/rezwanulrimel/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://github.com/rezwanulislamrimel"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---
<p align="center"><i>Maintained by Rezwanul Rimel © 2026</i></p>
