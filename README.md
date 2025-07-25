# 🛡️ AI Secure API — Host a Secure Inference Model in AWS

This project demonstrates how to **securely deploy an AI inference API** on AWS using a pre-trained LLM (e.g., GPT-J or Mistral), FastAPI, Docker, and Terraform. It is designed for cloud security, DevOps, and AI engineering learners and professionals.

---

## 🎯 Project Goals

- Deploy a FastAPI-based inference server for a pre-trained language model
- Use AWS EC2, IAM, VPC, and S3 with secure networking and logging
- Manage all infrastructure using Terraform
- Follow cloud security best practices (WAF-ready, IAM roles, SGs)
- Optional: Scan deployment with Wiz to identify misconfigurations

---

## ✅ Prerequisites

- AWS Account with Free Tier access
- IAM User with Administrator or scoped EC2/S3/IAM access
- AWS CLI installed and configured (`aws configure`)
- Terraform installed (v1.6+ recommended)
- Docker installed
- Python 3.10+ with `virtualenv`
- SSH key added to GitHub (for repo access)

---

## 📁 Project Structure


ai-secure-api/
├── infra/ # Terraform code
├── app/ # FastAPI app and model server
├── Dockerfile # Container for FastAPI app
├── .env.example # Sample environment variables
└── README.md # This file

yaml
Copy
Edit

---

## 🧱 Infrastructure (Terraform)

- VPC with `10.0.0.0/16` CIDR
- Public subnet with internet access (`10.0.1.0/24`)
- Internet Gateway + Route Table
- Security Group allowing HTTPS (port 443)
- EC2 instance with optional IAM role
- S3 bucket for model storage/logging

---

## 🚀 Deployment Steps

1. Clone this repo  
2. Configure AWS CLI  
3. Set up infrastructure:
   ```bash
   cd infra
   terraform init
   terraform apply
