sername` and `password` |
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
├── 05a-launch-e
---

## Resume Value

> This project demonstrates practical experience in securing application credentials using AWS services, making it valuable for **Cloud Security**, **DevOps**, and **Cloud Engineering** roles.
