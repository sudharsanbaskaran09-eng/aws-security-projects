# CloudTrai
AWS Console Activity
        ↓
CloudTrail captures events
        ↓
Audit logs generated
        ↓
Logs stored in Amazon S3
        ↓
Security auditing & monitoring
```

---

# Project Steps

| Step | Task |
|---|---|
| 01 | Create S3 Bucket for Logs |
| 02 | Enable AWS CloudTrail |
| 03 | View CloudTrail Event History |
| 04 | Verify Logs Stored in S3 |

---

# CloudTrail Event Monitoring

CloudTrail records:
- AWS Console activity
- API calls
- IAM actions
- Resource modifications
- Security events
- User activities

---

# Security Importance

CloudTrail is widely used for:

- Security auditing
- Incident investigation
- Compliance monitoring
- Forensic analysis
- Governance tracking
- Suspicious activity monitoring

---

# S3 Log Storage

CloudTrail delivers:
- compressed `.json.gz` log files
- timestamped audit records
- activity history
- AWS event details

into secure Amazon S3 storage.

---

# Screenshots

```text
screenshots/
├── 01-create-s3-bucket.png
├── 02-enable-cloudtrail.png
├── 03-cloudtrail-event-history.png
└── 04-cloudtrail-logs-in-s3.png
```

---

# Expected Output

## CloudTrail Event History

- AWS API calls
- Resource activities
- User actions
- Console events

## S3 Log Storage

- `.json.gz` CloudTrail logs
- Timestamped audit records
- Centralized log repository

---

# Skills Demonstrated

- AWS CloudTrail
- Audit Logging
- Security Monitoring
- AWS Event Tracking
- Cloud Governance
- Log Management
- SIEM Concepts
- Cloud Security Operations

---

# Learning Outcome

This project helped in understanding:

- How AWS audit logging works
- Event monitoring workflows
- Cloud activity tracking
- Secure log storage
- Security governance concepts
- SIEM-style monitoring basics

---

# Resume Value

This project demonstrates practical knowledge of:

- Cloud Security Monitoring
- AWS Audit Logging
- Security Operations
- Governance & Compliance
- SIEM-style workflows

Useful for:
- Cloud Security Engineer roles
- SOC Analyst roles
- DevSecOps roles
- AWS Security roles

---

# Future Improvements

- Integrate CloudWatch monitoring
- Add SNS alert notifications
- Query logs using Amazon Athena
- Integrate external SIEM tools
- Add automated threat alerts

---

# Conclusion

This project successfully demonstrates how to implement centralized audit logging and security event monitoring using AWS CloudTrail and Amazon S3.

It showcases practical cloud security monitoring and governance workflows using AWS native services.

---

# Author

## Sudharsan B
