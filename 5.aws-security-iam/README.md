<!-- ======================================================================= -->
<!--                          CLOUD SECURITY WITH AWS IAM                    -->
<!-- ======================================================================= -->

<h1 align="center">☁️🔐 Cloud Security with <code>AWS IAM</code></1>

<p align="center">
  <img src="https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/IAM-Security-blue?logo=awslambda&logoColor=white" />
  <img src="https://img.shields.io/badge/Terraform-IaC-purple?logo=terraform&logoColor=white" />
  <img src="https://img.shields.io/badge/CloudTrail-Audit-green?logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/GuardDuty-Threat%20Detection-red?logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/STS-Temporary%20Creds-yellow?logo=amazonaws&logoColor=black" />
  <img src="https://img.shields.io/badge/Organizations-SSO-brightgreen?logo=amazonaws&logoColor=white" />
</p>

> **Landing-Page Hook:** *Secure every identity, policy, and permission in your AWS estate—then prove it with hands-on code, Terraform blueprints, and audit automations. Dive in and see exactly how I did it, step by step!*

---

## 🎯 Skills Demonstrated

| ![IAM](https://img.icons8.com/color/48/000000/key-security.png) **Identity & Access Management** | ![Terraform](https://img.icons8.com/color/48/000000/terraform.png) **Infrastructure as Code** | ![GuardDuty](https://img.icons8.com/color/48/000000/bug.png) **Threat Detection** | ![CloudTrail](https://img.icons8.com/color/48/000000/compass.png) **Cloud Auditing** | ![Python](https://img.icons8.com/color/48/000000/python.png) **Python Automation** | ![DevSecOps](https://img.icons8.com/color/48/000000/shield.png) **DevSecOps** |
|---|---|---|---|---|---|

---

## 🚀 Project Overview

Cloud identities are the Achilles’ heel of most breaches. In this project I designed **least-privilege AWS IAM**, codified governance with **Terraform**, automated evidence collection using **CloudTrail**, and wired continuous detection via **GuardDuty**—all documented from zero to production.

<!-- ![Architecture Diagram](https://github.com/your-username/your-repo/assets/architecture.svg) 
*High-level architecture—download the repo for full diagrams!*
-->
---

## 📚 Documentation & Walk-Through

* **Full Project Documentation:** [Securing Identities in AWS IAM – Design & Implementation](https://mega.nz/file/PqBn2YwA#dY903Udy6RjaHOtsN_ynpvNf5_-eDiKUUaO0CqDjqD0)

---

## 🛠️ What I Built

| Feature | Highlights |
|---------|------------|
| **Zero-Trust IAM Roles** | Role segmentation, tagging strategy, enforced MFA, cross-account boundary policies |
| **Terraform Modules** | Modular IAM roles, S3 CloudTrail bucket with SSE-KMS, GuardDuty enablement |
| **Automated Evidence** | Lambda Python script to snapshot IAM policies and push to S3 nightly |
| **GuardRails & SCPs** | AWS Organizations Service Control Policies to block wildcards in IAM actions |
| **Continuous Audit** | CloudTrail Lake queries + Athena dashboard to detect privilege escalation |

---

## ✨ Learning Outcomes

- Crafted production-grade **least-privilege policies** with condition keys, resource scoping, and deny-overrides.  
- Mastered **Terraform best practices** (remote state, workspaces, modules).  
- Integrated **GuardDuty** findings into Slack via EventBridge for real-time alerts.  
- Automated **evidence generation** and compliance reporting for auditors.  

---

## 🧰 Technologies Used

AWS IAM - AWS Organizations - AWS STS - AWS CloudTrail - AWS GuardDuty - Terraform - Python 3.11 - GitHub Actions - Athena - KMS - S3


---

---

## 📈 Results

| Metric | Before Hardening | After Hardening |
|--------|------------------|-----------------|
| IAM Policies with “*” | 27 | **0** |
| GuardDuty Findings / 30 days | 12 | **0** |
| Average Time-to-Provision (mins) | 45 | **5** |

---

## ✒️ Author

**Suvrajeet Banerjee**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?logo=linkedin)](https://www.linkedin.com/in/suvrajeet/)

---

## 🔗 Useful Links

- **Project Documentation** – *Securing Identities in AWS IAM – Design & Implementation*  
  <https://mega.nz/file/PqBn2YwA#dY903Udy6RjaHOtsN_ynpvNf5_-eDiKUUaO0CqDjqD0>

- **Community Showcase Post** – *Cloud Security with AWS IAM & AWS Analytics with QuickSight*  
  <https://community.nextwork.org/c/celebrations/cloud-security-with-aws-iam-aws-analytics-with-quicksight>

<!-- Blog Article – uncomment & replace when published -->
- **Blog:** 🔐*Mastering AWS IAM: How to Control EC2 Access Like a Pro [Part-5]*  
  <https://dev.to/suvrajeet/mastering-aws-iam-how-to-control-ec2-access-like-a-pro-part-5-4gd0>


---

## 🙏 Acknowledgments
This learning journey was powered & supported by NextWork's structured approach to cloud education, which made breaking down complex concepts into digestable-byte-sized-hands-on practical accessible through systematic skill building & clear-actionable steps.

This write-up is based on - NextWork's - Cloud Security with AWS IAM Challenge!

Give it a try: <https://learn.nextwork.org/projects/aws-security-iam>

---
