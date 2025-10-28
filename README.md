📘 Overview

This project demonstrates a CI/CD pipeline using Jenkins and Docker.
The pipeline automates the process of building, testing, and deploying a simple web application.

🛠️ Technologies Used

Python (Flask) – for the web app

Docker – for containerization

Jenkins – for continuous integration and deployment

GitHub – for version control

⚙️ Project Structure
jenkins-cicd-pipeline/
│
├── app.py            # Simple Flask app
├── Dockerfile        # Docker build instructions
├── Jenkinsfile       # Jenkins pipeline script
└── README.md         # Project documentation

🚀 Steps to Run
1. Build Docker Image
docker build -t jenkins-cicd-app .

2. Run Container
docker run -p 5000:5000 jenkins-cicd-app

3. Jenkins Pipeline

Open Jenkins → Create a new Pipeline project

Add your GitHub repository link

Jenkins will automatically use the Jenkinsfile

Click Build Now to run the pipeline

📦 Pipeline Stages

Build – Builds Docker image

Test – Runs simple test

Deploy – Runs container

✅ Output

Visit:

http://localhost:5000


You’ll see:

Hello from Jenkins Pipeline!
