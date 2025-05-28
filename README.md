# 🌐 GO REST API Testing with Newman

This repository contains automated tests for the **GO REST API**, executed using **Postman** and reported through **Newman**.

## 📦 Project Overview

- REST API: [GO REST API](https://gorest.co.in/)
- Tool: [Postman](https://www.postman.com/)
- CLI Runner: [Newman](https://www.npmjs.com/package/newman)
- Report Format: HTML (via `newman-reporter-htmlextra`)

## 🧪 What's Included

- Postman collection file: `GoRest.postman_collection.json`
- Postman environment file: `GoRest.postman_environment.json`
- Newman run command
- HTML report generated from test execution

## 🚀 How to Run the Tests

Make sure you have **Node.js** and **Newman** installed.

### 1. Install Newman and HTML Reporter

```bash
npm install -g newman newman-reporter-htmlextra
newman run GoRestCol.postman_collection.json -r htmlextra --reporter-htmlextra-browserTitle "GoRest Bearer Token API Report" --reporter-htmlextra-title "GoRest API Result"

### Folder Structure
.
├── GoRest.postman_collection.json
├── newman (folder)
└── README.md

Make sure the access token for the GO REST API is valid and up-to-date in the environment file.
Customize the Postman collection to suit different endpoints or test cases.
