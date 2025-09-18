# 🏦 BankApp DevSecOps on AWS EKS using ArgoCD

🚀 A **production-ready Bank Application** featuring **CI/CD, security, and observability** — deployed on **AWS EKS** using modern **DevSecOps practices**.  

---

## 🛠️ Tech Stack  

- 📂 **GitHub** → Code hosting & version control  
- 📦 **Docker** → Containerization  
- 🔄 **Jenkins** → Continuous Integration (CI)  
- 🛡️ **OWASP** → Dependency vulnerability checks  
- 🧹 **SonarQube** → Code quality & static analysis  
- 🔍 **Trivy** → Filesystem & container image scanning  
- 🚀 **ArgoCD** → Continuous Delivery (CD)  
- ☸️ **AWS EKS** → Kubernetes orchestration  
- 📜 **Helm** → Manifest templating & deployment  
- 📊 **Grafana & Prometheus** → Monitoring & visualization  

---

## 📖 Application Overview  

This project demonstrates **end-to-end automation** for deploying a **secure, scalable, and highly available Spring Boot–based banking application** on **AWS EKS**.  

✔️ Integrated quality checks  
✔️ Vulnerability scanning  
✔️ Monitored production environments  
✔️ Security & compliance at every stage  

🔗 The architecture ensures **speed, reliability, and security** throughout the deployment lifecycle.  

---

## 🏗️ Architecture  

Below is the high-level architecture of the project:  

Developer → GitHub → Jenkins CI → SonarQube + OWASP + Trivy → DockerHub
↓
ArgoCD → AWS EKS (Kubernetes + Helm)
↓
Prometheus + Grafana → Observability & Monitoring

- **CI/CD**: Jenkins automates build, test, scan, and image push.  
- **Security**: OWASP, SonarQube, and Trivy ensure code and container security.  
- **CD**: ArgoCD automates deployment into AWS EKS.  
- **Observability**: Prometheus collects metrics, Grafana provides dashboards.  

---

## ⚡ Requirements & Notes  

- 🌍 **Deployment Region** → `us-east-1` (North Virginia)  
- 👤 **AWS Access** → Root account / IAM user with sufficient permissions  
- 🔑 **System Access** → Requires `sudo` privileges  
- 🔒 **Security Groups** → Ensure ports are open as per reference screenshot  
- 🖥️ **Master Node** → `t2.medium` (29GB storage)  
- ⚙️ **Pre-setup** → AWS CLI, `kubectl`, and `eksctl` configured before cluster creation  

---

## 📸 Key Screenshots  

- 💻 **Application UI** <br><br>
      <img width="1901" height="1134" alt="Screenshot 2025-09-17 143700" src="https://github.com/user-attachments/assets/7c7869fe-28ff-4b2d-8b0c-fa89717b845d" />

- ☸️ **AWS EKS Console** <br><br> 
      <img width="1915" height="994" alt="Screenshot 2025-09-18 174939" src="https://github.com/user-attachments/assets/4d6cf6d4-d6ed-4728-9849-186449a157c8" />
      <img width="1909" height="987" alt="Screenshot 2025-09-18 174857" src="https://github.com/user-attachments/assets/cbad7647-a9c8-4eaf-af39-3fc7f2954bd2" />

- 🚀 **ArgoCD Dashboard** <br><br>
      <img width="1919" height="1052" alt="Screenshot 2025-09-17 142928" src="https://github.com/user-attachments/assets/c9d13bf9-afa7-4f01-b17f-411c542e7f81" />
      <img width="1864" height="995" alt="Screenshot 2025-09-18 174243" src="https://github.com/user-attachments/assets/9576349c-0d58-4201-947e-25418b499b50" />
      <img width="1611" height="867" alt="Screenshot 2025-09-18 173731" src="https://github.com/user-attachments/assets/ef581ef4-7284-4ec0-8232-ae106f3dc7c0" />

- 🐳 **DockerHub Repository** <br><br>
      <img width="1919" height="870" alt="Screenshot 2025-09-18 174225" src="https://github.com/user-attachments/assets/1e142899-1512-4371-8d9b-4ed4aa02f162" />

- ⚙️ **Jenkins CI Pipeline** <br><br>
      <img width="1915" height="1094" alt="Screenshot 2025-09-18 174058" src="https://github.com/user-attachments/assets/9ec98510-d988-4c27-8f4f-73b0b853d8fe" />

- 📊 **Grafana Monitoring** <br><br>
      <img width="1916" height="1085" alt="Screenshot 2025-09-18 173310" src="https://github.com/user-attachments/assets/9c9595dd-2df5-439a-af0e-e9fb73b77a72" />
      <img width="1913" height="994" alt="Screenshot 2025-09-18 173936" src="https://github.com/user-attachments/assets/c47c3f7e-d1d8-4439-a559-96c51072f1be" />
      <img width="1903" height="992" alt="Screenshot 2025-09-18 174022" src="https://github.com/user-attachments/assets/099b613f-007c-4438-9615-58fc516bd305" />

---

✨ With this setup, you get a **bank-grade application** deployed with **modern DevSecOps practices** — combining **automation, security, and observability** on the cloud.  

