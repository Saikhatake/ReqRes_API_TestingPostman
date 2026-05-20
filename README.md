# 🧪 ReqRes REST API — QA Testing Project
 
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Tool](https://img.shields.io/badge/Tool-Postman-orange)
![TestCases](https://img.shields.io/badge/Test%20Cases-22-blue)
![PassRate](https://img.shields.io/badge/Pass%20Rate-100%25-success)
 
---
 
## 📌 Project Overview
 
Manual API testing project for the **ReqRes public REST API** (https://reqres.in).  
This project covers end-to-end validation of user management and authentication endpoints using **Postman**.  
Test cases include positive, negative, and boundary value scenarios across all major HTTP methods.
 
---
 
## 👤 Tester Details
 
| Field | Details |
|---|---|
| **Name** | Sai Khatake |
| **Email** | saikhatake@gmail.com |
| **GitHub** | github.com/Saikhatake |
| **Tool Used** | Postman |
| **Test Environment** | https://reqres.in |
| **Execution Date** | May 2026 |
 
---
 
## 🎯 Scope of Testing
 
| Module | Method | Endpoint |
|---|---|---|
| List Users | GET | /api/users?page=1 |
| Single User | GET | /api/users/{id} |
| User Not Found | GET | /api/users/23 |
| Create User | POST | /api/users |
| Login Successful | POST | /api/login |
| Login Unsuccessful | POST | /api/login |
| Update User | PUT | /api/users/{id} |
| Delete User | DELETE | /api/users/{id} |
 
---
 
## 🧾 Test Case Summary
 
| Module | Total TCs | Passed | Failed |
|---|---|---|---|
| List Users | 3 | 3 | 0 |
| Single User | 3 | 3 | 0 |
| Create User | 4 | 4 | 0 |
| Login | 6 | 6 | 0 |
| Update User | 3 | 3 | 0 |
| Delete User | 3 | 3 | 0 |
| **Total** | **22** | **22** | **0** |
 
---
 
## 🔍 Testing Types Covered
 
- ✅ Positive Testing — valid inputs and expected success responses
- ✅ Negative Testing — missing fields, invalid IDs, wrong credentials
- ✅ Boundary Value Analysis — first/last user IDs, empty bodies
- ✅ Status Code Validation — 200, 201, 204, 400, 404
- ✅ Response Body Validation — field presence, data types, values
- ✅ Error Message Validation — correct error text for bad requests
---
 
## 🐛 Bugs Found
 
| Bug ID | Module | Bug Title | Severity |
|---|---|---|---|
| BUG001 | Create User | Empty request body returns 201 instead of 400 | Medium |
| BUG002 | Delete User | Non-existent user ID returns 204 instead of 404 | Low |
 
> Full bug details with steps to reproduce are in the Excel test case file.
 
---
 
## 📁 Repository Structure
 
```
api-testing-reqres/
│
├── README.md                                  ← You are here
├── ReqRes_API_TestCases_SaiKhatake.xlsx       ← All 22 test cases + bug report + summary
└── ReqRes_API_Testing.postman_collection.json ← Postman collection (import and run)
```
 
---
 
## 🚀 How to Use This Project
 
### Run the Postman Collection
1. Download `ReqRes_API_Testing.postman_collection.json` from this repo
2. Open **Postman**
3. Click **Import** → select the downloaded JSON file
4. Go to **Collections** → open `ReqRes API Testing`
5. Add your API key in the Collection headers under `x-api-key`
6. Run each request and verify against expected results in the Excel file
### View Test Cases
1. Download `ReqRes_API_TestCases_SaiKhatake.xlsx`
2. Open in Microsoft Excel or Google Sheets
3. Three sheets inside:
   - **Test Cases** — all 22 test cases with results
   - **Bug Report** — defects found with steps to reproduce
   - **Summary** — execution metrics and pass rate
---
 
## 🛠️ Tools & Technologies
 
| Tool | Purpose |
|---|---|
| Postman | API request execution and validation |
| Microsoft Excel | Test case documentation and bug reporting |
| ReqRes.in | Public REST API used as application under test |
| Chrome Browser | Manual verification of API docs |
| Git & GitHub | Version control and project hosting |
 
---
 
## 📚 Key Learnings
 
- Understood GET, POST, PUT, DELETE HTTP methods and when each is used
- Validated status codes (200, 201, 204, 400, 404) and their meanings
- Identified that ReqRes API accepts empty request bodies without validation (potential API design issue)
- Practiced writing structured bug reports with severity and priority classification
- Applied Boundary Value Analysis to API input fields (user IDs, empty bodies)
---
 
## 🔗 Connect With Me
 
- 📧 Email: saikhatake@gmail.com
- 💼 LinkedIn: linkedin.com/in/saikhatake
- 🐙 GitHub: github.com/Saikhatake
