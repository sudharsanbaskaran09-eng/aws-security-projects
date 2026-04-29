# Project 1: IAM Role & Policy Management

A hands-on AWS Security project focused on implementing secure Identity and Access Management (IAM) practices using IAM Users, Custom Policies, IAM Roles, and Multi-Factor Authentication (MFA).

This project demonstrates how to control access to AWS resources using the **Principle of Least Privilege**, where users and services receive only the permissions they need.

---

## Project Objective

Build a secure AWS environment where:

- IAM users have restricted access based on job role
- EC2 instances access AWS services using IAM Roles
- Custom IAM policies are created for fine-grained permissions
- MFA is enabled for stronger account security
- No hardcoded AWS credentials are used

---

## Services Used

- AWS IAM
- Amazon EC2
- Amazon S3
- AWS CLI

---

## Key Features

- Create IAM User with limited permissions
- Attach AWS managed and custom IAM policies
- Create IAM Role for EC2
- Use temporary credentials instead of access keys
- Enable Multi-Factor Authentication
- Test secure access using AWS CLI

---

## Architecture

```text
IAM User (developer-user)
        ↓
Custom / Managed Policy
        ↓
Limited Access to AWS Resources

EC2 Instance
        ↓
IAM Role
        ↓
Temporary Credentials
        ↓
Amazon S3 Access
