<div align="center">

#  Employee REST API Automation
### Postman · Newman · JavaScript

[![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)](https://www.postman.com/)
[![Newman](https://img.shields.io/badge/Newman-CLI_Runner-EF5B25?style=for-the-badge&logo=node.js&logoColor=white)](https://github.com/postmanlabs/newman)
[![Node.js](https://img.shields.io/badge/Node.js-Required-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Tests](https://img.shields.io/badge/Test_Cases-20%2B_Automated-brightgreen?style=for-the-badge)](#-testing-coverage)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)](#)

<br/>

> A production-ready **API Testing Framework** for an Employee Management System — featuring 20+ automated test cases, dynamic data generation, and CLI-based execution built for seamless CI/CD integration.

<br/>

[ Documentation](#-api-documentation) · [ Quick Start](#-quick-start) · [ Test Coverage](#-testing-coverage) · [ Project Structure](#-project-structure)

</div>

---

##  Table of Contents

1. [Project Overview](#-project-overview)
2. [Tech Stack](#%EF%B8%8F-tech-stack)
3. [Testing Coverage](#-testing-coverage)
4. [Test Execution Summary](#-test-execution-summary)
5. [Quick Start](#-quick-start)
6. [API Documentation](#-api-documentation)
7. [Project Structure](#-project-structure)
8. [Author](#-author)

---

## 🧩 Project Overview

This project provides a full-featured automation suite for testing a RESTful Employee Management API. It covers the complete lifecycle of API interactions — from authentication and CRUD operations to schema validation and negative test scenarios — all executable from the command line with rich HTML reporting.

**Key Highlights:**
- ✅ 20+ test scenarios covering happy paths and edge cases
- 🔄 Dynamic test data via JavaScript `Math.random()` and `Date.now()`
- 📊 HTML dashboard reports generated automatically via `htmlextra`
- 🔗 CI/CD-ready Newman CLI execution
- 📋 Full Postman API documentation published online

---

##  Tech Stack

| Layer | Tool | Purpose |
| :--- | :--- | :--- |
| **Test Design** | Postman | Collection & environment management |
| **CLI Execution** | Newman | Automated, headless test runs |
| **Scripting** | JavaScript | Pre-request scripts & assertions |
| **Reporting** | newman-reporter-htmlextra | Visual HTML dashboards |
| **Documentation** | Postman Documenter | Published API reference |

---

## 🧪 Testing Coverage

###  1. Authentication & Security

| Type | Scenario |
| :--- | :--- |
| ✅ Positive | Valid login with JWT/token retrieval |
| ❌ Negative | Unauthorized access handling |
| ❌ Negative | Invalid credential validation |

###  2. Dynamic CRUD Operations

| Operation | Details |
| :--- | :--- |
| **Create** | Auto-creates **5 employees** using randomized data per run |
| **Read** | Retrieves single and paginated employee records |
| **Update** | Selectively patches Mobile Number and Position fields |
| **Delete** | Validates resource removal and confirms `404` post-deletion |

###  3. Validation & Assertions

| Assertion Type | Description |
| :--- | :--- |
| **Schema Validation** | Verifies JSON structure and field data types |
| **Query Parameters** | Filters records and validates total count via query strings |
| **Status Codes** | Enforces REST standards — `200`, `201`, `400`, `401`, `404` |
| **Response Time** | Flags responses exceeding acceptable thresholds |

---

##  Test Execution Summary

| Metric | Details |
| :--- | :--- |
| **Total Test Cases** | `20+` Scenarios |
| **Execution Mode** | Newman CLI |
| **Environment** | `TestEnv` with dynamic variable injection |
| **Data Strategy** | Pre-request scripts with randomized payloads |
| **Report Formats** | CLI output + HTML dashboard (htmlextra) |

---

##  Quick Start

### Prerequisites

Ensure [Node.js](https://nodejs.org/) is installed, then install Newman and the HTML reporter globally:

```bash
npm install -g newman
npm install -g newman-reporter-htmlextra
```

### Clone the Repository

```bash
git clone https://github.com/rezwanulislamrimel/<your-repo-name>.git
cd <your-repo-name>
```

### Run Tests

**CLI output only:**
```bash
newman run collections/employee_api_tests.json \
  -e environments/test_env.json
```

**CLI + HTML report (recommended):**
```bash
newman run collections/employee_api_tests.json \
  -e environments/test_env.json \
  -r cli,htmlextra \
  --reporter-htmlextra-export ./reports/automation_dashboard.html
```

>  After execution, open `reports/automation_dashboard.html` in your browser to view the full interactive test dashboard.

---

##  API Documentation

| Resource | Link |
| :--- | :--- |
| 📘 Postman API Docs | [View Online](https://documenter.getpostman.com/view/25113210/2sB3BLhSC1) |
| 📦 Postman Collection | [`collections/employee_api_tests.json`](./collections/employee_api_tests.json) |
| ⚙️ Environment File | [`environments/test_env.json`](./environments/test_env.json) |
| 📸 Report Screenshots | [`/screenshots`](./screenshots) |

> [!NOTE]
> All test data is dynamically generated per run using JavaScript `Math.random()` and `Date.now()` inside Postman pre-request scripts, ensuring no duplicate or stale data across executions.

---

##  Project Structure

```
📦 employee-api-automation
├── 📂 collections
│   └── employee_api_tests.json       # Postman collection export
├── 📂 environments
│   └── test_env.json                 # Environment variables
├── 📂 reports
│   └── automation_dashboard.html     # Generated HTML report
├── 📂 screenshots
│   ├── cli_output.png                # Newman CLI execution proof
│   └── html_report_dashboard.png     # HTML report preview
└── 📄 README.md
```

---

## 👤 Author

**Rezwanul Islam**
*SQA Engineer · API Automation Specialist*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rezwanulrimel/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/rezwanulislamrimel)

---

<div align="center">

*Maintained with ❤️ by Rezwanul Rimel · © 2026*

</div>
