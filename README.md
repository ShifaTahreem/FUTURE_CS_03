# FUTURE_CS_03
# API Security Risk Analysis

## Cyber Security Internship – Future Interns

**Name:** Shifa Tahreem

**CIN:** FIT/JUN26/CS9072

**Task:** Cyber Security Task 3

**Project:** API Security Risk Analysis

---

## Project Overview:

This project focuses on performing a read-only API Security Risk Analysis on a public testing API. The assessment evaluates authentication mechanisms, authorization controls, exposed data, rate-limiting controls, and input validation practices. The objective is to identify common API security risks, assess their business impact, and recommend security improvements based on industry best practices.

---

## Objectives:

* Analyze a public API using Postman
* Review authentication requirements
* Assess authorization controls
* Identify excessive data exposure
* Review rate-limiting indicators
* Evaluate input validation practices
* Classify identified risks
* Document findings professionally
* Recommend security improvements

---

## Tools & Resources Used:

### API Testing

* Postman
* Browser Developer Tools

### Documentation

* Microsoft Word
* PDF Export
* GitHub

### API Tested

* JSONPlaceholder API
* https://jsonplaceholder.typicode.com

---

## Methodology:

1. Reviewed API documentation
2. Tested publicly accessible endpoints
3. Inspected requests and responses
4. Analyzed exposed data fields
5. Evaluated authentication controls
6. Reviewed authorization mechanisms
7. Assessed evidence of rate limiting
8. Identified security risks
9. Assigned severity ratings
10. Developed remediation recommendations

---

## Endpoints Tested:

### Users Endpoint

GET /users

### Single User Endpoint

GET /users/1

### Posts Endpoint

GET /posts

### Comments Endpoint

GET /comments

---

## Security Findings:

### F-01 Missing Authentication Controls:

**Risk Level:** Medium

API endpoints returned data without requiring authentication credentials, API keys, or bearer tokens.

---

### F-02 Excessive Data Exposure:

**Risk Level:** Medium

User records exposed multiple information fields including names, email addresses, phone numbers, company details, and addresses.

---

### F-03 Missing Rate Limiting Evidence:

**Risk Level:** Medium

No visible evidence of API rate-limiting controls was identified during testing.

---

### F-04 Predictable Resource Access:

**Risk Level:** Low-Medium

Resources were accessible using predictable sequential identifiers such as:

* /users/1
* /users/2
* /users/3

---

### F-05 Input Validation Not Evident:

**Risk Level:** Low

Input validation controls were not clearly visible during testing or documented in the tested endpoints.

---

## Risk Classification Summary:

| Finding | Description                     | Severity   |
| ------- | ------------------------------- | ---------- |
| F-01    | Missing Authentication Controls | Medium     |
| F-02    | Excessive Data Exposure         | Medium     |
| F-03    | Missing Rate Limiting Evidence  | Medium     |
| F-04    | Predictable Resource Access     | Low-Medium |
| F-05    | Input Validation Not Evident    | Low        |

---

## Business Impact:

The identified observations demonstrate common API security weaknesses that could expose sensitive information, increase abuse risks, and weaken access control mechanisms if present in a production environment.

Potential impacts include:

* Unauthorized access to information
* Increased data exposure risks
* Resource abuse and service degradation
* Weak access control enforcement
* Increased attack surface

---

## Security Recommendations:

* Implement OAuth 2.0 or JWT authentication
* Enforce authorization checks for resource access
* Apply data minimization principles
* Implement API rate limiting and throttling
* Validate all user input on the server side
* Monitor and log suspicious API activity
* Follow OWASP API Security best practices

---

## OWASP API Security Alignment:

| Finding | Related OWASP API Security Concern                    |
| ------- | ----------------------------------------------------- |
| F-01    | Broken Authentication                                 |
| F-02    | Excessive Data Exposure                               |
| F-03    | Unrestricted Resource Consumption                     |
| F-04    | Broken Object Level Authorization                     |
| F-05    | Security Misconfiguration / Improper Input Validation |

---

## Repository Contents:

```text
FUTURE_CS_03
│
├── README.md
│
├── API_Security_Risk_Analysis_Report.pdf
│  
└── Evidence
    ├── users_endpoint.png
    ├── user1_endpoint.png
    ├── headers_tab.png
    ├── posts_endpoint.png
    └── comments_endpoint.png
```

---

## Skills Gained:

* API Security Assessment
* Authentication Analysis
* Authorization Review
* Risk Identification
* Security Documentation
* SaaS Security Fundamentals
* Security Reporting
* OWASP API Security Concepts

---

## Conclusion:

The project successfully identified common API security concerns including missing authentication controls, excessive data exposure, lack of visible rate-limiting mechanisms, predictable resource access patterns, and insufficient evidence of input validation. The assessment demonstrates practical API security analysis skills and highlights the importance of secure API design in modern SaaS applications.

---

## Disclaimer:

This assessment was conducted exclusively on a publicly available testing API using ethical, read-only techniques. No exploitation, bypass attempts, denial-of-service testing, or unauthorized activities were performed.

---

## Author:

**Shifa Tahreem**

Cyber Security Intern

Future Interns | June 2026
