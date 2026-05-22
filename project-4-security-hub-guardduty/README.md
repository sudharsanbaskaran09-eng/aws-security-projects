# AWS Security Hub & GuardDuty Monitoring

A hands-on AWS Security project focused on implementing threat detection, centralized security monitoring, and compliance visibility using Amazon GuardDuty and AWS Security Hub.

This project demonstrates how security teams monitor AWS environments for suspicious activity and aggregate findings into a centralized security dashboard.

---

# Project Objective

The goal of this project is to:

- Enable AWS threat detection services
- Monitor suspicious activities in AWS
- Aggregate findings into a centralized dashboard
- Analyze security findings and severity levels
- Understand cloud security monitoring workflows
- Implement compliance visibility using AWS Security Hub

---

# AWS Services Used

| Service | Purpose |
|---|---|
| Amazon GuardDuty | Threat detection and monitoring |
| AWS Security Hub | Centralized security findings dashboard |
| AWS CloudTrail | Event logging and activity monitoring |
| IAM | Identity and access monitoring |

---

# Architecture Overview

```text
AWS Account Activity
        ↓
CloudTrail Logs
        ↓
Amazon GuardDuty
        ↓
Threat Detection & Findings
        ↓
AWS Security Hub
        ↓
Centralized Security Dashboard
```

---

# Key Features

- Threat detection using GuardDuty
- Centralized monitoring using Security Hub
- Security findings aggregation
- Severity-based alert visibility
- Compliance monitoring
- Security posture visibility
- Cloud security operations workflow

---

# Project Workflow

```text
AWS Activity
      ↓
CloudTrail Events
      ↓
GuardDuty analyzes logs
      ↓
Threat findings generated
      ↓
Security Hub aggregates findings
      ↓
Security dashboard & compliance visibility
```

---

# Project Steps

| Step | Task |
|---|---|
| 01 | Enable Amazon GuardDuty |
| 02 | Enable AWS Security Hub |
| 03 | Generate/View Security Findings |
| 04 | Analyze Security Hub Findings |
| 05 | Review Security Dashboard & Compliance |

---

# Threat Monitoring Components

## Amazon GuardDuty

GuardDuty continuously monitors:
- CloudTrail events
- DNS logs
- AWS account behavior
- Network activity

to detect:
- suspicious API calls
- credential compromise
- unusual account behavior
- malicious activity

---

# AWS Security Hub

Security Hub provides:
- centralized security dashboard
- compliance visibility
- severity categorization
- aggregated security findings
- monitoring across AWS services

---

# Findings Severity Levels

| Severity | Meaning |
|---|---|
| Critical | Immediate security risk |
| High | Serious threat detected |
| Medium | Potential security issue |
| Low | Minor issue or warning |
| Informational | Monitoring insight |

---

# Screenshots

```text
screenshots/
├── 01-enable-guardduty.png
├── 02-enable-security-hub.png
├── 03-guardduty-findings-dashboard.png
├── 04-security-hub-findings.png
└── 05-security-score-dashboard.png
```

---

# Expected Output

## Security Hub Dashboard

- Critical findings
- High severity alerts
- Compliance overview
- Security monitoring dashboard
- Threat visibility

---

# Skills Demonstrated

- AWS GuardDuty
- AWS Security Hub
- Threat Detection
- Security Monitoring
- Cloud Security Operations
- Compliance Visibility
- AWS Security Best Practices

---

# Learning Outcome

This project helped in understanding:

- How AWS detects suspicious activities
- Cloud threat monitoring workflows
- Security findings aggregation
- Compliance monitoring
- Real-world cloud security operations

---

# Resume Value

This project demonstrates practical knowledge of:

- Cloud Security Monitoring
- Threat Detection Systems
- Security Operations
- AWS Native Security Services
- Compliance Visibility

Useful for:
- Cloud Security Engineer roles
- SOC Analyst roles
- DevSecOps roles
- AWS Security roles

---

# Future Improvements

- Integrate SNS alerts
- Add automated remediation
- Enable Security Hub automation
- Add AWS Config integration
- Create custom GuardDuty filters

---

# Conclusion

This project successfully demonstrates how to implement centralized cloud security monitoring and threat detection using AWS GuardDuty and AWS Security Hub.

It showcases practical cloud security operations and security visibility workflows using AWS native security services.

---

# Author

## Sudharsan B
