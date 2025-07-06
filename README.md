<div align="center">
  <img src="./public/assets/DevSecOps.png" alt="Logo" width="100%" height="100%">

  <br>
  <a href="http://netflix-clone-with-tmdb-using-react-mui.vercel.app/">
    <img src="./public/assets/netflix-logo.png" alt="Logo" width="100" height="32">
  </a>
</div>

<br />

<div align="center">
  <img src="./public/assets/home-page.png" alt="Logo" width="100%" height="100%">
  <p align="center">Home Page</p>
</div>

# DevSecOps Netflix Clone Project 🎬🚀

A Netflix-style application deployed and secured using industry-standard DevSecOps practices. This project demonstrates CI/CD pipelines, containerization, vulnerability scanning, and monitoring on AWS infrastructure.

---

## 📸 Screenshots

View screenshot folder for project outputs.

---

## 🎯 Key Features

✅ React-based Netflix Clone with TMDB API  
✅ Dockerized application with Image pushed to DockerHub  
✅ Jenkins CI/CD Pipeline automating build, test & deployment  
✅ Integrated **SonarQube** for Code Quality and Security  
✅ Container Vulnerability Scanning with **Trivy**  
✅ Static Dependency Scanning with **OWASP Dependency-Check**  
✅ Application deployed inside Docker Containers  
✅ Real-time Monitoring with **Prometheus & Grafana**  
✅ Infrastructure hosted on AWS EC2 Ubuntu Instances  
✅ Follows complete DevSecOps Lifecycle  

---

## 🛠️ Tools & Technologies Used

- **Docker & DockerHub**
- **Jenkins**
- **SonarQube**
- **OWASP Dependency-Check**
- **Trivy**
- **Prometheus**
- **Grafana**
- **AWS EC2**
- **Git & GitHub**
- **React, TypeScript**
---

## 🗂️ Project Structure

DevSecOps-Netflix-Clone-Project/
├── Dockerfile
├── Jenkins Pipeline Script
├── Kubernetes/
├── src/
├── public/
├── screenshots/
├── README.md
└── ...

---
🔧 System Architecture

[ GitHub ] --> [ Jenkins (CI/CD) ] --> [ DockerHub ]
                           |               |
                       [ SonarQube ]   [ Trivy Scan ]
                           |
                     [ Kubernetes (EKS) ]
                           |
                [ ArgoCD (GitOps) ] --> [ Prometheus & Grafana ]
----

## ⚡ CI/CD Pipeline Overview

The Jenkins pipeline performs:

1. Workspace Cleanup  
2. Code Checkout from GitHub  
3. SonarQube Analysis  
4. Quality Gate Validation  
5. Dependency Install  
6. OWASP FS Scan  
7. Trivy Image Scan  
8. Docker Build & Push to DockerHub  
9. Container Deployment  
10. Monitoring Setup  

---

## 🚀 How to Run Locally

```bash
# Clone the repo
git clone https://github.com/IMASHM/DevSecOps-Netflix-Clone-project.git

# Navigate to project
cd DevSecOps-Netflix-Clone-project

# Build Docker Image (Replace <API_KEY>)
docker build --build-arg TMDB_V3_API_KEY=<your-api-key> -t netflix .

# Run the container
docker run -d --name netflix -p 8081:80 netflix

# Access the app
http://<your-ec2-ip>:8081
📊 Monitoring Access
Prometheus: http://<your-ec2-ip>:9090

Grafana: http://<your-ec2-ip>:3000 (Default credentials: admin / admin)

📢 Credits
This project was built as a learning showcase integrating DevSecOps tools and practices.

