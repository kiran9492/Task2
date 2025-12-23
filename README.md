OBJECTIVE :
Set up a basic Jenkins pipeline to automate the process of building and deploying a web application using Docker.

Tools Used
●  Jenkins – for CI/CD pipeline automation
●  Docker – for containerizing and deploying the application
●  GitHub – for source code management
●  Linux Server (EC2 / VM) – for hosting Jenkins and Docker

Task Implementation :
●  Created a Linux server and installed Jenkins and Docker
●  Configured Jenkins with required permissions to run Docker commands
●  Developed a Dockerfile to containerize the web application
●  Created a Jenkins pipeline (Jenkinsfile) with stages to:
●  Checkout source code from GitHub
●  Build a Docker image
●  Stop and remove existing containers
●  Deploy the application using Docker
Successfully executed the pipeline and deployed the web application

README.md :
# Jenkins CI/CD Pipeline for Web Application Deployment
## 📌 Project Overview
This project demonstrates how to set up a basic Jenkins CI/CD pipeline to automate the process of building and deploying a web application using Docker.

The pipeline pulls source code from GitHub, builds a Docker image, and deploys the application as a running container on a server.

## 🎯 Objective
- Automate build and deployment of a web application
- Use Jenkins pipeline for CI/CD
- Containerize the application using Docker
  
## 🛠️ Tools & Technologies Used
- Jenkins
- Docker
- Git & GitHub
- Linux Server (EC2 / VM)

## 🏗️ Project Architecture
1. Developer pushes code to GitHub
2. Jenkins pulls the source code
3. Jenkins builds a Docker image
4. Existing container is stopped (if any)
5. New container is deployed automatically

Jenkins Pipeline :
Automates build and deployment. 

How to Run the Project:
1️⃣ Server Setup
  ● Launch a Linux server
  ● Install Jenkins and Docker
  ● Add Jenkins user to Docker group
-sudo usermod -aG docker jenkins
-sudo systemctl restart jenkins

2️⃣ Jenkins Job Configuration
    1. Create a Pipeline job
    2. Select Pipeline script from SCM
    3. Add GitHub repository URL
    4. Set branch to main
    5. Save and build

  <img width="1366" height="768" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/b42dabc6-034d-4076-ae1e-619d1d249358" />



<img width="1366" height="768" alt="Screenshot (72)" src="https://github.com/user-attachments/assets/55395d42-1bf3-4833-83e6-3f9a7878559a" />











