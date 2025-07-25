<!-- =============================== -->
<!--        HOST ON AMAZON S3       -->
<!-- =============================== -->

<p align="center">
  <!-- Skill Badges -->
  <img src="https://img.sh.io/badge/AWS-S3-blue?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/CloudFront-CDN-orange?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Route_53-DNS-green?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/IaC-Terraform-purple?style=for-the-badge&logo=terraform&logoColor=white"/>
  <img src="https://img.shields.io/badge/CI%2FCD-GitHub_Actions-2ea44f?style=for-the-badge&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/Automation-Boto3-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Security-ACM_TLS-red?style=for-the-badge&logo=letsencrypt&logoColor=white"/>
  <img src="https://img.shields.io/badge/Static_Website-Hosting-yellow?style=for-the-badge&logo=html5&logoColor=white"/>
</p>

# 🛰️ Host a Website on Amazon S3
Deploy a **serverless**, **blazing-fast**, and **cost-effective** static website in minutes — from _zero_ to **global**.

> _Learned & implemented from the official AWS documentation and the in-depth [“Host Your First Website on AWS S3 – From Zero to Live in 45 Minutes”](https://dev.to/suvrajeet/host-your-first-website-on-aws-s3-from-zero-to-live-in-45-minutes-part-3-db6) blog._

---

## 🎯 What You’ll Build
1. **S3 Bucket** – Static hosting with public-read policy  
2. **CloudFront CDN** – HTTPS, caching & edge delivery  
3. **Custom Domain (Route 53)** – Point DNS to CloudFront  
4. **CI/CD Pipeline** – Auto-deploy on every `git push` via GitHub Actions  
5. **IaC** – Reproducible infrastructure with Terraform & Boto3 automation  

---
---

## 🧑‍💻 Key Learnings
- **Object Storage at Scale:** Leveraged Amazon S3 to store and serve static assets with versioning and lifecycle rules.  
- **Global Delivery:** Configured CloudFront for low-latency edge caching, custom error pages, and HTTP/2.  
- **Secure TLS Everywhere:** Automated ACM certificates (us-east-1) and enforced HTTPS via CloudFront.  
- **Domain Management:** Used Route 53 alias records for root and sub-domain routing.  
- **Infrastructure as Code:** Wrote reusable Terraform modules and parametrized variables for multi-environment deployment.  
- **Zero-Downtime Deploys:** Integrated GitHub Actions with OIDC authentication to sync S3 and invalidate CloudFront.  
- **Policy-as-Code:** Applied least-privilege bucket policies and OAI/OAC for private S3 origins.  
- **Automated Testing:** Added workflow steps for `terraform fmt`, `plan`, and `validate` to gate PRs.

---

## 🛠️ Step-by-Step Guide

| Step | Action | Key CLI / Console |
|------|--------|------------------|
| 1 | Create versioned S3 bucket | `aws s3 mb s3://<your-domain>` |
| 2 | Disable **Block All Public Access** | Console › Permissions |
| 3 | Enable **Static Website Hosting** (`index.html`, `error.html`) | Console › Properties |
| 4 | Attach bucket policy for public-read | `aws s3api put-bucket-policy ...` |
| 5 | Upload site assets | `aws s3 sync ./public s3://<bucket>` |
| 6 | Request ACM certificate for domain | Console › Certificate Manager |
| 7 | Create CloudFront distribution (OAI/OAC) | Console › CloudFront |
| 8 | Point Route 53 A/AAAA records to distribution | Console › Route 53 |
| 9 | Automate deploys with GitHub Actions | `.github/workflows/deploy.yml` |

---

## 📚 Further Reading
* **Full Documentation** → [Host a Website on Amazon S3 (PDF)](https://mega.nz/file/X3AjCSwQ#9kcMqdw_paBD4wgWpgGT5SNphxZzr62N9yjbTYmFFXs)  
* **45-Minute Walk-through Blog** → [Host Your First Website on AWS S3 – Part 3](https://dev.to/suvrajeet/host-your-first-website-on-aws-s3-from-zero-to-live-in-45-minutes-part-3-db6)

---

## 🗺️ Roadmap
- [ ] GitHub Pages fallback workflow  
- [ ] CloudFront Functions for A/B testing  
- [ ] Lambda@Edge for security headers  

---

## 🤝 Contributing
PRs and issues are welcome! Please review `CONTRIBUTING.md` before submitting.

---

## 📜 License
Distributed under the MIT License. See `LICENSE` for details.

---

## 🔗 Stay Connected
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/suvrajeet/)

---

## 📬 Related Resources
* **Hosted initial static website using S3 – community post**  
  <https://community.nextwork.org/c/celebrations/hosted-nextwork-s-initial-static-website-using-s3>

<!-- blog link = Host Your First Website on AWS S3 – Part 3 -->

---

## 🙏 Acknowledgments  
This learning journey was powered & supported by NextWork's structured approach to cloud education, which made breaking down complex concepts into digestable-byte-sized hands-on practice accessible through systematic skill building & clear-actionable steps.

This blog is based on - NextWork's - title=above !

Give it a try → <https://learn.nextwork.org/projects/aws-host-a-website-on-s3?track=high>

<p align="center">© 2025 – <strong>Suvrajeet Banerjee</strong></p>
