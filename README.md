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


