
 # 🚀Node.js CI/CD Pipeline using Jenkins on AWS EC2

This project demonstrates a **Node.js web application** deployed automatically using a **Jenkins CI/CD pipeline** hosted on an **AWS EC2 instance**.

---

 # Project Overview

- **Language/Framework:** Node.js (Express.js)
- **CI/CD Tool:** Jenkins
- **Server:** AWS EC2 (Ubuntu)
- **Version Control:** GitHub
- **Build Tool:** npm (depending on project setup)
- **Pipeline Type:** Declarative Jenkins Pipeline (Jenkinsfile)

---

---
## AWS EC2 Instance (Ubuntu)
![](./image/Screenshot%202025-11-06%20000206.png)
## ⚙️ Prerequisites

Before you begin, make sure you have the following installed:
- **Node.js & npm**
- **Jenkins Server** (installed and running on EC2)
- **Git** (for fetching code from GitHub)

---

## 🖥️ Jenkins Setup on EC2

### 1️⃣ Install Jenkins
```bash
sudo apt update
sudo apt install jenkins -y
sudo systemctl enable jenkins
sudo systemctl start jenkins
```
## Jenkinsfile

✅ Updated the Jenkinsfile in VS Code to automate the build and deployment process of the Node.js application.
![](./image/Screenshot%202025-11-06%20000541.png)


## 🔗Connect GitHub Repository

1) Go to Jenkins Dashboard → New Item → Pipeline

2) Add your GitHub Repository URL

3) Select "Pipeline script from SCM"

4) Choose Git
```bash
Paste your repository URL
https://github.com/RohanShinde2421/node-app.git
```

5) Set branch (main)
### Image of connect github repository
![](./image/Screenshot%202025-11-08%20162828.png)


## Output
✅ Successfully built and deployed the Node.js application using Jenkins on AWS EC2. The pipeline ran smoothly, completing all stages — checkout, clone, upload, install, and start — without errors. 
The screenshot shows the final successful build execution, confirming the CI/CD setup is working perfectly.

![](./image/Screenshot%202025-11-08%20163726.png)

![](./image/Screenshot%202025-11-06%20000133.png)

## Conclusion
The Node-App-Deployment project successfully automated the build and deployment of a Node.js application using Jenkins on AWS EC2. The CI/CD pipeline worked efficiently, pulling code from GitHub, building it, and deploying automatically. This setup ensures faster updates, smooth delivery, and reliable continuous integration and deployment.