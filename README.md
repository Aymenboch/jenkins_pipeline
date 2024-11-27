jenkins_pipeline
A fully automated CI/CD pipeline built using Jenkins, Docker, and Kubernetes. This project automates the process of code retrieval, Docker image building, pushing to DockerHub, and deploying to a Kubernetes cluster.

🚀 Features:
Jenkins running in a Docker container to automate the CI/CD process.
Minikube as a local Kubernetes cluster running inside a container.
Docker to build and push containerized applications to DockerHub.
Kubernetes YAML files for deployment in the Minikube cluster.
GitHub Actions triggers the pipeline automatically when code is updated.
🛠️ Setup Instructions:
1. Set up Docker and Minikube:
Install Docker: Docker Installation Guide
Install Minikube: Minikube Installation Guide
2. Run Jenkins in Docker:
Pull the Jenkins image and run it in a container:

docker pull jenkins/jenkins:lts
docker run -d -p 8080:8080 -p 50000:50000 --name jenkins jenkins/jenkins:lts
3. Configure Jenkins:
Add DockerHub and GitHub credentials in Jenkins:
DockerHub credentials: For pushing Docker images.
GitHub credentials: To fetch code from your repository.
Install necessary Jenkins plugins:
Docker Pipeline
Kubernetes CLI
Git Plugin
4. Set up the Pipeline:
Create a Jenkins pipeline with a Jenkinsfile:
Retrieve code from GitHub.
Build Docker image and push to DockerHub.
Deploy to Kubernetes using Minikube.
💡 Why I'm Proud of This Project:
This project provided hands-on experience with CI/CD automation, containerization, and Kubernetes orchestration. It allowed me to strengthen my skills in automating workflows, troubleshooting container networking issues, and managing infrastructure. The project also helped me gain a deeper understanding of how to integrate various DevOps tools in a seamless process.

🎯 Goal:
I am actively seeking an internship where I can apply and expand my knowledge in DevOps, cloud technologies, and automation. I am passionate about improving deployment workflows and working with cutting-edge technologies.
