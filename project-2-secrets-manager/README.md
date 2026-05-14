## Services Used

| Category | Service |
|---|---|
| Security | AWS Secrets Manager |
| Identity | AWS IAM |
| Compute | Amazon EC2 |
| CLI | AWS CLI |

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
 AWS Secrets Manager usage
- IAM policy creation
  

