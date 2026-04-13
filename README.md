# AWS Security Projects Portfolio

A hands-on collection of 6 AWS Security projects built on Amazon Web Services (AWS), progressing from beginner to advanced level — built as part of my Cloud Security Engineer learning journey.

---

## About Me

- Fresher | Aspiring Cloud Security Engineer
- Hands-on AWS Security & IAM projects
- AWS IAM | Monitoring | Threat Detection | Web Security
- Chennai, India

---

## Projects

| # | Project | Services Used | Level |
|---|---------|--------------|-------|
| 1 | [IAM Role & Policy Management](./project-1-iam-role-policy-management) | IAM, EC2, S3 | Beginner |
| 2 | [AWS Secrets Manager for Credential Storage](./project-2-secrets-manager) | Secrets Manager, IAM, Lambda | Beginner |
| 3 | [API Gateway Security](./project-3-api-gateway-security) | API Gateway, Cognito, IAM, WAF | Intermediate |
| 4 | [AWS Security Hub & GuardDuty](./project-4-security-hub-guardduty) | Security Hub, GuardDuty, IAM | Intermediate |
| 5 | [CloudTrail Logging & SIEM Integration](./project-5-cloudtrail-siem) | CloudTrail, CloudWatch, S3, IAM | Advanced |
| 6 | [AWS WAF for Application Security](./project-6-aws-waf-security) | AWS WAF, ALB, CloudFront, Shield | Advanced |

---

## Architecture Overview

```text
User / Admin Access
        ↓
AWS IAM              — Identity & Access Control
        ↓
Monitoring Layer     — CloudTrail / GuardDuty / Security Hub
        ↓
Protection Layer     — WAF / API Gateway Security
        ↓
Secrets Layer        — Secrets Manager
        ↓
Storage & Logs       — S3 / CloudWatch
```
## Tech Stack

| Category | Tools |
|----------|-------|
| Cloud | Amazon Web Services (AWS) |
| Security | IAM, WAF, GuardDuty, Security Hub |
| Monitoring | CloudTrail, CloudWatch |
| Identity | IAM Roles, Policies, MFA |
| Secrets | AWS Secrets Manager |
| API Security | API Gateway, Cognito |
| Logging | S3, CloudWatch Logs |
| Networking | ALB, CloudFront |

## How to Set Up

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
## Skills Demonstrated
- IAM Role & Policy Creation
- Least Privilege Access Control
- Credential Protection using Secrets Manager
- API Authentication & Authorization
- Threat Detection & Security Monitoring
- Log Auditing & Governance
- Web Application Firewall Rules
- Cloud Security Best Practices

---

## Certifications (Planned / In Progress)

- [ ] AWS Certified Cloud Practitioner
- [ ] AWS Certified Security – Specialty
- [ ] AWS Certified Solutions Architect – Associate

---

## Screenshots

Every project contains a dedicated screenshots folder with complete step-by-step implementation images.

---

## Connect

- LinkedIn: https://linkedin.com/in/sudharsan-baskaran-95443925a
- GitHub: https://github.com/sudharsanbaskaran09-eng
