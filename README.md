# 🌐 Shaun Barnett – Cloud Engineer Portfolio (Azure Static Website)

This project hosts my professional Cloud Engineer portfolio as a fully deployed **Azure Static Website** with automated CI/CD using **GitHub Actions** and secure **OIDC authentication**.

The website serves as a live, interactive version of my CV, showcasing:
- Cloud engineering expertise
- Azure administration skills
- IT infrastructure experience
- Certifications and career history
- Projects, skills, and contact links

🔗 **Live Portfolio:**  
https://shaunstaticweb.z6.web.core.windows.net/

---

## 🚀 Technology Stack

### **Azure Services**
- Azure Storage Account (Static Website Hosting)
- Azure Blob Storage (`$web` container)
- Microsoft Entra ID App Registration
- Federated Identity Credentials (OIDC)
- Azure RBAC (Storage Blob Data Contributor)

### **CI/CD**
- GitHub Actions workflow
- OIDC login (passwordless & secure)
- Automated deployment to Azure on each push to `main`

---

## 🛠️ Features of This Portfolio

### **Frontend**
- Clean, modern single‑page CV website
- HTML5, CSS3, responsive design
- Certification logos
- Animated skill bars
- Contact links
- Professional layout suitable for employers

### **Backend / Cloud**
- Fully serverless
- Zero compute cost
- Extremely low hosting cost (pennies per month)
- Secure GitHub → Azure deployment
- No secrets stored in GitHub (OIDC)

---

## 🔧 CI/CD Pipeline Summary

Deployment is automated through `.github/workflows/deploy.yml`:

1. GitHub authenticates to Azure via OIDC  
2. Workflow uploads all website files to `$web` container  
3. Azure instantly updates the live site  
4. No manual deployment required  

This follows Microsoft’s recommended best practice for cloud deployments.

---

## 🧩 File Structure


.
├── index.html        # Main CV website
├── README.md         # Project documentation
└── .github/
└── workflows/
└── deploy.yml

---

## 🔒 Security

This project uses **OpenID Connect (OIDC)** to authenticate GitHub → Azure:

✔ No passwords or secrets stored  
✔ Temporary token issuance  
✔ Federated identity credentials  
✔ Least‑privilege “Blob Data Contributor” RBAC  

This is the secure modern alternative to access keys.

---

## 💡 Why This Project?

This portfolio demonstrates practical Azure skills directly relevant to a Cloud Engineer role:

- Azure Storage hosting
- Identity & Access (Entra ID)
- Azure Networking basics
- Cloud automation pipelines
- RBAC and access security
- GitHub Actions CI/CD
- Static website best practices

It also provides a professional online portfolio for employers and recruiters.

---

## 🙋‍♂️ Author

**Shaun Barnett**  
Cloud Engineer | Azure Administrator | IT Infrastructure Specialist  

🔗 GitHub: https://github.com/shaunbarnett  
🔗 LinkedIn: https://www.linkedin.com/in/shaun-barnett-446b32215/  
📧 Email: shaunbarnett1@hotmail.com  

---

## 📬 Feedback

If you'd like to use this template or collaborate, feel free to reach out.
