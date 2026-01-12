1.	Introduction
This document explains the complete process of deploying a Java Web Application using Docker and Tomcat. It covers required commands, their purpose, and why each step is used. This approach uses a multi-stage Docker build to optimize image size and performance.
2. Prerequisites 
• Amazon EC2 (Amazon Linux 2023) 
• Docker Installed 
• Git Installed 
• Java-based Web Application (Maven project) 
• Internet Access 
3. Install Git 
Command: 
sudo yum install git -y
<img width="916" height="469" alt="image" src="https://github.com/user-attachments/assets/300c8ca5-de3d-4327-b081-a1b8859eddf8" />
Purpose: 
Git is required to clone the project repository from GitHub. 
5. Clone Project Repository 
Command: 
git clone https://github.com/ramyachetty/web-app.git
<img width="916" height="416" alt="image" src="https://github.com/user-attachments/assets/3f81a750-567c-4a70-a923-1e500edf5903" />
Purpose: 
This downloads the project source code into the EC2 instance. 
7. Navigate into Project Directory 
Command: 
cd web-app
<img width="916" height="438" alt="image" src="https://github.com/user-attachments/assets/4404593c-1fdc-4037-9db4-a50daeaa46ba" />

Purpose: 
Access project files such as Dockerfile, pom.xml, and source code. 
9. Dockerfile (Multi-Stage Build Explanation) 
Stage 1 (Build Stage) 
10. Build Docker Image 
Command: 
docker build -t webapp . 
<img width="916" height="455" alt="image" src="https://github.com/user-attachments/assets/75b1a7e2-3211-4562-94dc-91080da6254c" />

Purpose: 
Creates a Docker image using instructions defined in Dockerfile. 
11. Run Docker Container 
Command: 
docker run -d -p 80:8080 --name webapp webapp 
<img width="916" height="438" alt="image" src="https://github.com/user-attachments/assets/ac168fa8-5d5e-4da4-9d4e-afdf2e494b4b" />

Purpose: 
Runs the application container and maps port 8080 inside container to port 80 on host. 
12. Verify Running Container 
Command: 
docker ps 
Purpose: 
Checks whether the container is running successfully. 
13. Access Application 
URL: 
http://ip -address 
Purpose: 
Opens deployed Java web application in browser. 
<img width="916" height="406" alt="image" src="https://github.com/user-attachments/assets/314b6546-7a3b-4091-be7b-cd312142e939" />
14. Logs Verification 
Command: 
docker logs webapp 
<img width="916" height="450" alt="image" src="https://github.com/user-attachments/assets/2446c569-8fc7-4194-96da-a4b1e268e5ea" />
Purpose: 
Used for debugging and verifying application startup logs. 
15. Conclusion 
This deployment uses Docker multi-stage builds for optimized performance, ensures clean 
separation of build and runtime environments, and enables scalable deployment using 
containers.
