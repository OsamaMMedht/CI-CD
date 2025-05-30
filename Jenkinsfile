pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/OsamaMMedht/CI-CD.git'
            }
        }

        stage('Verify Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t node-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat 'docker run -d -p 3000:3000 --name my-node-app node-app'
            }
        }

    }

    post {
        failure {
            echo 'Build failed.'
        }
        success {
            echo 'Build and run succeeded.'
        }
    }
}