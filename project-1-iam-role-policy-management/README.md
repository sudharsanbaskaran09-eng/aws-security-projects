# Project 1: IAM Role & Policy Management

A hands-on AWS Security project focused on implementing secure Identity and Access Management (IAM) using IAM Users, Policies, Roles, and Multi-Factor Authentication (MFA).

This project demonstrates how to secure AWS resources using the **Principle of Least Privilege**, ensuring users and services only receive the permissions they need.

---

## Project Objective

Build a secure AWS environment where:

- IAM users have controlled access
- EC2 instances securely access S3 using IAM Roles
- Custom policies provide fine-grained permissions
- MFA protects user accounts
- No hardcoded AWS credentials are used

---

## Services Used

| Service | Purpose |
|---|---|
| AWS IAM | Identity & Access Management |
| Amazon EC2 | Virtual machine with IAM Role attached |
| Amazon S3 | Storage accessed via temporary credentials |
| AWS CLI | Verify access and test permissions |

---

## Key Features

- Create IAM User with restricted permissions
- Attach AWS managed policies
- Create custom IAM policies
- Create IAM Role for EC2
- Use temporary credentials instead of access keys
- Enable MFA for stronger security
- Verify access using AWS CLI

---

## Architecture

```text
Developer User
      ↓
IAM User
      ↓
Managed / Custom Policy
      ↓
Limited AWS Access

EC2 Instance
      ↓
IAM Role
      ↓
Temporary Credentials
      ↓
Amazon S3 Access
```

---

## Project Steps

| Step | Action |
|---|---|
| 01 | Open AWS IAM Console |
| 02 | Create IAM User (`developer-user`) |
| 03 | Attach `AmazonS3ReadOnlyAccess` policy |
| 04 | Create Custom IAM Policy |
| 05 | Create IAM Role for EC2 |
| 06 | Launch EC2 with IAM Role attached |
| 07 | Verify access using AWS CLI |
| 08 | Enable MFA for User Security |

### Step 07 — Verify Access via AWS CLI

```bash
aws s3 ls
```

---

## IAM Policy Example

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket",
        "s3:GetObject"
      ],
      "Resource": "*"
    }
  ]
}
```

---

## Security Concepts Demonstrated

| Concept | Description |
|---|---|
| Identity & Access Management | Controlled user and service access |
| Least Privilege Principle | Users/services get only what they need |
| Role-Based Access Control | Permissions via roles, not hardcoded keys |
| Temporary Credentials | EC2 uses STS-issued short-lived tokens |
| MFA Security | Extra authentication layer for users |
| Cloud Governance | Policy-driven access management |

---

## Screenshots

```text
screenshots/
├── 01-open-iam-dashboard.png
├── 02-create-iam-user.png
├── 03-attach-s3-policy-user.png
├── 04-create-custom-policy.png
├── 05-create-iam-role-ec2.png
├── 06-launch-ec2-with-role.png
├── 07-test-role-s3-access.png
└── 08-enable-mfa-user.png
```

---

## Outcome

Successfully secured AWS access using IAM Users, Policies, Roles, and MFA — demonstrating real-world cloud security practices with zero hardcoded credentials.

---

## Skills Gained

- AWS IAM Administration
- Access Control Management
- Security Hardening
- EC2 IAM Role Usage
- Cloud Security Fundamentals

---

## Resume Value

> This project demonstrates practical AWS security knowledge valuable for **Cloud Engineer**, **DevOps**, and **Security** roles.
