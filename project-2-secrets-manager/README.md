# Project 2: AWS Secrets Manager for Credential Storage

A hands-on AWS Security project demonstrating how to securely store and retrieve sensitive information such as usernames, passwords, and API keys using AWS Secrets Manager.

This project eliminates hardcoded credentials and uses IAM Roles for secure, scalable access.

---

## Project Objective

Build a secure system where:

- Sensitive data is stored in AWS Secrets Manager
- Access is controlled using IAM policies
- EC2 retrieves secrets securely using IAM Role
- No credentials are exposed in code or configuration

---

## Services Used

| Category | Service |
|---|---|
| Security | AWS Secrets Manager |
| Identity | AWS IAM |
| Compute | Amazon EC2 |
| CLI | AWS CLI |

---

## Key Features

- Secure storage of credentials
- IAM-based access control
- EC2 Role-based authentication
- No hardcoded secrets
- Real-world cloud security implementation

---

## Architecture

```text
Secrets Manager
      ↓
Stores Credentials
      ↓
IAM Role
      ↓
EC2 Instance
      ↓
Secure Retrieval using AWS CLI
```

---

## Project Steps

| Step | Action |
|---|---|
| 01 | Open AWS Secrets Manager |
| 02 | Create Secret (type: Other) — add `username` and `password` |
| 03 | Configure Secret — name it `my-app-credentials` |
| 04 | Create IAM Policy — allow `secretsmanager:GetSecretValue` |
| 05 | Create IAM Role for EC2 — attach `SecretsManagerReadPolicy` |
| 06 | Launch EC2 Instance — Amazon Linux 2023, t2.micro |
| 07 | Attach `EC2-Secrets-Access-Role` to EC2 |
| 08 | Retrieve secret using AWS CLI |

### Step 08 — Retrieve Secret via AWS CLI

```bash
aws secretsmanager get-secret-value \
  --secret-id my-app-credentials \
  --region us-east-1
```

---

## IAM Policy Example

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": ["secretsmanager:GetSecretValue"],
      "Resource": "*"
    }
  ]
}
```

---

## Screenshots

```text
screenshots/
├── 01-open-secrets-manager.png
├── 02-create-secret.png
├── 03-secret-created.png
├── 04-create-policy.png
├── 05-create-role.png
├── 05a-launch-ec2.png
├── 06-attach-role.png
└── 07-fetch-secret.png
```

---

## Outcome

- Credentials stored securely in AWS Secrets Manager
- No exposure of sensitive data in code or config
- IAM controls access effectively
- EC2 retrieves secrets using role-based authentication

---

## Skills Gained

- AWS Secrets Manager usage
- IAM policy creation
- Role-based access control
- Secure credential management
- Cloud security best practices

---

## Resume Value

> This project demonstrates practical experience in securing application credentials using AWS services, making it valuable for **Cloud Security**, **DevOps**, and **Cloud Engineering** roles.
