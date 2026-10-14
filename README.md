# Automated Infrastructure Provisioning and Kubernetes Deployment⁠

This repository contains a practical DevOps learning project that documents how to build and deploy an application through a basic CI/CD workflow using Jenkins, Maven, Ansible, Docker, Tomcat, and Kubernetes.


## Author

**roudayna kouka**

## Project Overview

The goal of this project is to provide a simple reference for setting up a DevOps delivery pipeline from source code build to containerized deployment. The repository is organized as implementation notes, job definitions, Dockerfiles, and Kubernetes manifests that can be reused as a starting point for labs, coursework, or personal practice.

## Main Topics Covered

- Git-based source workflow
- Jenkins installation and pipeline/job configuration
- Maven build integration
- Ansible automation for deployment tasks
- Docker image creation and container deployment
- Tomcat installation and application hosting
- Kubernetes deployment and service exposure

## Repository Structure

- `Ansible/`: Ansible installation and setup notes
- `Docker/`: Docker commands, installation steps, Docker Hub usage, and Dockerfile examples
- `Jenkins/`: Jenkins installation, plugin setup, Maven setup, and Ansible integration
- `Jenkins_Jobs/`: Sample Jenkins job documentation and automation files
- `Kubernetes/`: Kubernetes deployment, service, and cluster setup examples
- `Tomcat/`: Tomcat installation and configuration guidance

## Typical Workflow

1. Install and configure Jenkins.
2. Connect Jenkins to the source repository.
3. Build the application with Maven.
4. Package and transfer the generated artifact.
5. Build a Docker image for the application.
6. Deploy the image either to a Docker host or to Kubernetes.
7. Use Ansible where automation between servers is required.

## Important Files

- `Jenkins_Jobs/create-docker-image.yml`: builds the Docker image
- `Jenkins_Jobs/create-docker-container.yml`: runs the Docker container
- `Kubernetes/valaxy-deploy.yml`: sample Kubernetes deployment manifest
- `Kubernetes/valaxy-service.yml`: sample Kubernetes service manifest
- `Kubernetes/create-simple-devops-image.yml`: image build and push automation
- `Docker/tomcat_dockerfile`: basic Tomcat Docker image example

## Notes

- This repository is mainly documentation-driven and intended for learning and demonstration.
- Some files contain example hostnames, usernames, repository URLs, and image names that should be adjusted for your own environment before use.
- The deployment object names under Kubernetes and Ansible were left unchanged to avoid breaking the existing examples.

## Suggested Next Improvements

- Replace placeholder infrastructure values with environment-specific values
- Add a Jenkinsfile for pipeline-as-code
- Add a sample application source directory for end-to-end testing
- Add validation steps for Docker and Kubernetes deployments

## License

Use this repository for learning, practice, and customization in your own environment.
