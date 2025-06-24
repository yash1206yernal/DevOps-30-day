# Day 16 – Terraform Variables & Modules

This repository contains Terraform configurations for **Day 16** of the 30-Day DevOps Challenge. The main goal is to learn how to:

- Use **input variables** and **output values**
- Create and use a **custom reusable module** to provision an AWS S3 bucket

---

## ✅ What I Learned

- How to define input variables using `variables.tf`
- How to provide values using `terraform.tfvars`
- How to output values using `outputs.tf`
- How to encapsulate logic in reusable **Terraform modules**

---

## 🧱 Project Structure
day16-variables-modules/
├── main.tf # Root config calling the module
├── variables.tf # Input variables for the root module
├── terraform.tfvars # Values for the variables
├── outputs.tf # Outputs from the root module
└── modules/
└── s3_bucket/
├── main.tf # Logic to create an S3 bucket
├── variables.tf # Module input variable (bucket name)
└── outputs.tf # Module output (bucket name)

## 🛠 Technologies Used

- Terraform v1.x
- AWS S3
- VS Code
- Git + GitHub

---

