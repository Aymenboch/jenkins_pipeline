#jenkins_pipeline
This project demonstrates a fully automated CI/CD pipeline built using Jenkins, Docker, and Kubernetes. The pipeline retrieves code from a Git repository, builds a Docker image, pushes it to DockerHub, and deploys the application to a Kubernetes cluster managed by Minikube.

#Features:
Jenkins running in a Docker container to automate the CI/CD process.
Minikube as a local Kubernetes cluster in a container.
Docker for building and pushing containerized applications.
Kubernetes YAML files for deploying the application.

#Setup Instructions:
Set up Docker and Minikube:

Install Docker and Minikube to create a local Kubernetes cluster.
Run Jenkins in Docker:

Pull the Jenkins image and run it in a container:
docker pull jenkins/jenkins:lts  
docker run -d -p 8080:8080 -p 50000:50000 --name jenkins jenkins/jenkins:lts
Configure Jenkins:

Add DockerHub and GitHub credentials in Jenkins for authentication.
Install necessary plugins (e.g., Docker Pipeline, Kubernetes CLI, Git Plugin).
Set up the Pipeline:

Create a Jenkins pipeline with a Jenkinsfile that automates:
Code retrieval from GitHub.
Docker image build and push to DockerHub.
Kubernetes deployment using Minikube.
