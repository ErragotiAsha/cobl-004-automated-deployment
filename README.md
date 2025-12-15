# 🌐 COBL-004 – Automated Solution Customer Deployment

This repository implements **COBL-004 AWS Cloud Operations Competency – Support for Automated Solution Customer Deployment** using **AWS CloudFormation, S3, IAM, Lambda**, and **GitHub Actions**.  
The solution demonstrates automated customer deployment, cross-account resource provisioning, governance, and secure access.

---

## ⚙️ Prerequisites

Ensure the following are available before implementation:

- AWS Account  
- IAM User with CloudFormation, S3, IAM, and Lambda privileges  
- AWS CLI v2 installed and configured  
- GitHub Repository  
- Valid AWS access keys  
- Region correctly set (example: `ap-south-1`)  

---

## 🔐 Required GitHub Secrets

Create an IAM user and generate access keys.  
Add the following secrets to your GitHub repository:

**Path:**  
`GitHub → Repository Settings → Secrets & Variables → Actions → New Repository Secret`

| Secret Name             | Description                              |
|-------------------------|------------------------------------------|
| `AWS_ACCESS_KEY_ID`     | IAM user access key                        |
| `AWS_SECRET_ACCESS_KEY` | IAM user secret key                        |

---

## 📁 Project Structure

```text
cobl-004-automated-deployment/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── cloudformation/
│   └── simple-iac.yaml
├── docs/
│   └── COBL-004_Automated_Deployment_Guide.md
├── README.md

