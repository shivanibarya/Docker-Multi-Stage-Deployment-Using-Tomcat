📌 Project Title

CI/CD Pipeline for Java Web Application using Jenkins, Maven & Docker

📖 Project Description

This project demonstrates a complete CI/CD pipeline implementation for a Java-based web application.
The pipeline automates the process of code cloning, building, Docker image creation, pushing to Docker Hub, and container deployment using Jenkins.

The project is deployed on an AWS EC2 instance with Jenkins, Docker, Maven, Git, and Java 17 installed.

🛠️ Tools & Technologies Used

AWS EC2 – Virtual server

Jenkins – CI/CD automation

Docker – Containerization

Docker Hub – Image repository

Maven – Build automation

Git & GitHub – Version control

Java 17 (Amazon Corretto) – Application runtime

Linux (Amazon Linux 2023)

🔄 CI/CD Pipeline Workflow

Clone Code from GitHub repository

Build Application using Maven

Create Docker Image

Push Docker Image to Docker Hub

Deploy Application using Docker container

🧩 Jenkins Pipeline Stages.

Clone Code
<img width="1920" height="1080" alt="Screenshot (673)" src="https://github.com/user-attachments/assets/3abddda0-3411-47bb-9f49-572c125c1df4" />
Build Code

Docker Image Build
<img width="1920" height="1080" alt="Screenshot (674)" src="https://github.com/user-attachments/assets/9fd56989-81cf-407d-b481-faf92e79fe3d" />

Docker Image Push

Deploy Container
<img width="1920" height="1080" alt="Screenshot (675)" src="https://github.com/user-attachments/assets/57089124-09f3-443f-a0bc-aed3539ec70d" />

🚀 How to Run the Project

Launch an AWS EC2 instance

Install:

Java 17

Jenkins

Maven

Git

Docker

Start Jenkins and configure required plugins

Add Docker Hub credentials in Jenkins

Create a Pipeline job

Add the provided Jenkinsfile

Run the pipeline

<img width="1920" height="1080" alt="Screenshot (676)" src="https://github.com/user-attachments/assets/d683e69a-cebc-4d29-b611-907765c0163e" />

🐳 Docker Image

Docker Hub Repo: shivanibarya/webapp
<img width="1920" height="1080" alt="Screenshot (677)" src="https://github.com/user-attachments/assets/a52125bb-3256-4bed-ac3a-05227b6feed0" />
Tag: latest

📂 Repository Structure
.
├── src/

├── pom.xml

├── Dockerfile

├── Jenkinsfile

└── README.md

✅ Key Features

Fully automated CI/CD pipeline

Dockerized Java web application

Secure Docker Hub authentication

Zero manual deployment steps

Scalable and production-ready approach

🎯 Learning Outcomes

Practical CI/CD implementation

Jenkins declarative pipelines

Docker image lifecycle management

AWS EC2 server setup

DevOps automation best practices

👩‍💻 Author

Shivani Barya
MCA (Cloud Computing)
DevOps & Cloud Enthusiast

🔗 GitHub: https://github.com/shivanibarya
