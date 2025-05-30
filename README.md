# CI/CD with Jenkins and Docker on Windows and Linux

This project demonstrates a basic CI/CD pipeline using Jenkins and Docker running on a Windows machine.

## Pipeline Steps

1. **Clone**
   - Pulls source code from the GitHub repository (`main` branch)

2. **Build**
   - Builds a Docker image named `node-app` using the included Dockerfile

3. **Run**
   - Runs the Docker container and maps port `3000` to the host

## Project Structure
CI-CD/
│
├── Jenkinsfile # Pipeline definition
├── Dockerfile # Node.js container image setup
├── package.json # Node.js dependencies
└── index.js # Simple app entry point


## Prerequisites

- Windows 10/11 with WSL2 enabled
- Docker Desktop (with WSL2 backend)
- Jenkins installed and running as a Windows service
- Git installed and available in system PATH

## How to Run the Pipeline

1. Make sure Jenkins has Docker access (use a user with permissions)
2. Create a new pipeline project in Jenkins
3. Point the project to this GitHub repo
4. Make sure Jenkinsfile exists in the repo root
5. Run the pipeline from Jenkins UI

## Author

Osama Mohammed Medhat  
[LinkedIn Profile](https://www.linkedin.com/in/osama-mohamedmedhat)
