# AWS Security Projects Portfolio

> A hands-on collection of **7 AWS Security projects** progressing from beginner to advanced — built as part of my Cloud Security Engineer learning journey.

<br>

## 👤 About Me

- 🎓 Fresher | Aspiring Cloud Security Engineer
- 🛠️ Hands-on AWS Security & IAM projects
- 🔑 AWS IAM | Monitoring | Threat Detection | Governance | Web Security
- 📍 Chennai, India

<br>

## 📁 Projects Overview
 | Secrets Manager, IAM, Lambda | 🟢 Beginner |
| 3 | [API Gateway Security](./projectF, API Gateway, Shield | 🔴 Advanced |

<br>

## 🏗️ Architecture Overview

```text
User / Admin Access
        │
        ▼
┌───────────────────┐
│    AWS IAM        │  ← Identity & Access Control
└───────┬───────────┘
        │
        ▼
┌───────────────────┐
│ Monitoring Layer  │  ← CloudTrail / GuardDuty / Security Hub
└───────┬───────────┘
        │
        ▼
┌───────────────────┐
│ Governance Layer  │  ← AWS Config Compliance Monitoring
└───────┬───────────┘
        │
        ▼
┌───────────────────┐
│ Protection Layer  │  ← WAF / API Gateway Security
└───────┬───────────┘
        │
        ▼
┌───────────────────┐
│  Secrets Layer    │  ← Secrets Manager
└───────┬───────────┘
        │
        ▼
┌───────────────────┐
│ Storage & Logs    │  ← S3 / CloudWatch
└───────────────────┘
```

<br>

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| ☁️ Cloud | Amazon Web Services (AWS) |
| 🔒 Security | IAM, WAF, GuardDuty, Security Hub, AWS Config |
| 📊 Monitoring | CloudTrail, CloudWatch |
| 🪪 Identity | IAM Roles, Policies, MFA |
| 🔑 Secrets | AWS Secrets Manager |
| 🔌 API Security | API Gateway, Cognito |
| 📝 Logging | S3, CloudWatch Logs |
| 🌐 Networking | CloudFront, Shield |

<br>

## 📂 Repository Structure

```text
aws-security-projects/
├── README.md
├── project-1-iam-role-policy-management/
├── project-2-secrets-manager/
├── project-3-api-gateway-security/
├── project-4-security-hub-guardduty/
├── project-5-cloudtrail-siem/
├── project-6-aws-config-compliance-monitoring/
└── project-7-aws-waf-application-security/
```

<br>

## ⚙️ How to Set Up

### Prerequisites

- AWS Account
- Basic IAM knowledge
- AWS CLI installed
- Browser access to AWS Console

### Configure AWS CLI

```bash
aws configure
# Enter Access Key, Secret Key, Region, Output Format
```

> Each project folder contains its own detailed `README.md` with step-by-step setup instructions.

<br>

## ✅ Skills Demonstrated

- IAM Role & Policy Creation
- Least Privilege Access Control
- Credential Protection using Secrets Manager
- API Authentication & Authorization
- Threat Detection & Security Monitoring
- Log Auditing & Governance
- Compliance Monitoring using AWS Config
- Web Application Firewall Rules
- Cloud Security Best Practices

<br>

## 🏅 Certifications

- [x] AWS Certified Cloud Practitioner (CLF-C02)
- [ ] AWS Certified Security – Specialty *(In Progress)*
- [ ] AWS Certified Solutions Architect – Associate *(Planned)*

<br>

## 📸 Screenshots

Every project contains a dedicated `screenshots/` folder with complete step-by-step implementation images.

<br>

## 🤝 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Sudharsan_Baskaran-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/sudharsan-baskaran-95443925a)
[![GitHub](https://img.shields.io/badge/GitHub-sudharsanbaskaran09--eng-181717?style=for-the-badge&logo=github)](https://github.com/sudharsanbaskaran09-eng)
