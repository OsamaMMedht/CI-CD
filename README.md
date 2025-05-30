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

