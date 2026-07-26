# API Manual Testing – Fake Store API

Manual API testing project on the public [Fake Store API](https://fakestoreapi.com), built to demonstrate manual QA test design, execution, and defect reporting applied to REST APIs — prior to moving into API automation with REST Assured.

## Why this project

Coming from 6+ years of manual PBM/claims testing, this project translates that same test-design discipline (positive/negative scenarios, boundary cases, structured defect logging) to a REST API context, as a foundation before automating the same coverage.

## Project Metrics

| Metric | Value |
|---|---|
| Endpoints Tested | 5 |
| Test Cases Designed | 15 |
| Executed | 15 |
| Passed | 14 |
| Failed | 1 |
| Blocked | 0 |
| Sample Defects Logged | 2 |

## Repository Structure

```
API-Manual-Testing
│
├── README.md
├── LICENSE
├── .gitignore
├── Test Plan/
│   └── API_Test_Plan.docx
├── Test Cases/
│   └── API_Test_Cases.xlsx
├── Test Execution/
│   └── Test_Execution_Report.xlsx
├── Defect Report/
│   └── Defect_Log.xlsx
├── Postman Collection/
│   └── FakeStore_API.postman_collection.json
├── Evidence/
│   ├── GET_All_Products_200.png
│   ├── GET_Invalid_Product_200_EmptyBody.png
│   ├── POST_Create_Product_200.png
│   ├── PUT_Update_Product_200.png
│   └── DELETE_Product_200.png
└── Request Response Samples/
    ├── GET_Product_Request.txt
    ├── GET_Product_Response.json
    ├── POST_Product_Request.json
    └── POST_Product_Response.json
```

## Scope

**In scope:** GET Products, GET Single Product, POST Product, PUT Product, DELETE Product
**Out of scope:** Performance, Security, Automation (covered in a separate automation repo)

## Endpoints Covered

| Method | Endpoint |
|--------|----------|
| GET | /products |
| GET | /products/{id} |
| POST | /products |
| PUT | /products/{id} |
| DELETE | /products/{id} |

## API Validations

- HTTP Status Codes
- Response Body
- JSON Schema (Manual)
- Header Validation
- Data Type Validation
- Negative Testing
- CRUD Operations

## Tools Used

Postman · Excel · GitHub

## Next Step

The automation counterpart to this project — the API coverage automated with REST Assured — is built here: [hybrid-automation-framework](#)
