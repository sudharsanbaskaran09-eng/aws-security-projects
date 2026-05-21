# API Gateway Security using Cognito & AWS WAF

A hands-on AWS Security project focused on securing serverless APIs using Amazon API Gateway, AWS Lambda, Amazon Cognito JWT Authentication, and AWS WAF.

This project demonstrates how to build a protected API architecture using authentication, authorization, and web application firewall security controls in AWS.

---

# Project Objective

The goal of this project is to:

- Create a serverless backend using AWS Lambda
- Expose the backend securely using API Gateway
- Implement JWT authentication using Amazon Cognito
- Protect APIs from unauthorized access
- Add AWS WAF protection against malicious traffic
- Understand real-world API security architecture

---

# AWS Services Used

| Service | Purpose |
|---|---|
| AWS Lambda | Backend serverless compute |
| API Gateway | API management and routing |
| Amazon Cognito | User authentication and JWT token generation |
| AWS WAF | Web application firewall protection |
| IAM | Permissions and access management |

---

# Architecture Overview

```text
User Request
      ↓
AWS WAF
      ↓
API Gateway
      ↓
Cognito JWT Validation
      ↓
AWS Lambda
      ↓
Secure Response
```

---

# Features Implemented

- Secure HTTP API using API Gateway
- AWS Lambda backend integration
- Cognito User Pool authentication
- JWT Authorizer configuration
- Unauthorized request blocking
- AWS WAF managed security rules
- Protected serverless architecture

---

# Project Steps

| Step | Task |
|---|---|
| 01 | Create Lambda Function |
| 02 | Create API Gateway |
| 03 | Test Public API |
| 04 | Create Cognito User Pool |
| 05 | Create Test User |
| 06 | Configure JWT Authorizer |
| 07 | Attach Authorizer to API |
| 08 | Verify Unauthorized Access Blocking |
| 09 | Create AWS WAF Protection |

---

# Lambda Function Code

```python
def lambda_handler(event, context):
    return {
        "statusCode": 200,
        "body": "Hello from Secure API"
    }
```

---

# Security Flow

```text
User Login
      ↓
Amazon Cognito
      ↓
JWT Token Generated
      ↓
API Gateway Validates Token
      ↓
Lambda Executes
      ↓
Response Returned
```

---

# WAF Protection

AWS WAF was configured using AWS Managed Rules to help protect the API from:

- SQL Injection (SQLi)
- Cross-Site Scripting (XSS)
- Common web exploits
- Malicious requests
- Bad traffic patterns

---

# Output Verification

## Before Security

```text
Hello from Secure API
```

## After JWT Authorizer

```text
{
  "message": "Unauthorized"
}
```

This confirms that unauthorized users are blocked successfully.

---

# Screenshots

The project contains complete step-by-step screenshots inside the screenshots folder.

```text
screenshots/
├── 01-create-lambda.png
├── 02-create-api.png
├── 03-test-api.png
├── 04-create-cognito.png
├── 05-create-user.png
├── 06-create-authorizer.png
├── 07-attach-authorizer.png
├── 08-unauthorized.png
└── 09-create-waf.png
```

---

# Skills Demonstrated

- API Security
- JWT Authentication
- Cognito Integration
- AWS WAF Configuration
- Secure Serverless Architecture
- Authentication & Authorization
- Cloud Security Best Practices

---

# Learning Outcome

This project helped in understanding:

- How API Gateway secures APIs
- JWT token validation flow
- Cognito-based authentication
- WAF protection layers
- Real-world cloud security architecture

---

# Future Improvements

- Add custom WAF rules
- Enable API throttling
- Add CloudWatch logging
- Implement MFA authentication
- Integrate Security Hub monitoring

---

# Conclusion

This project successfully demonstrates how to secure serverless APIs in AWS using Cognito JWT authentication and AWS WAF protection.

It showcases practical cloud security implementation using modern AWS security services and serverless architecture.

---

# Author

## Sudharsan B
