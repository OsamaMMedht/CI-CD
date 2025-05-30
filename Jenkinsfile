pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git branch: 'main', url: 'https://github.com/OsamaMMedht/CI-CD.git'
      }
    }
    stage('Build') {
      steps {
        bat 'docker build -t node-app .'
      }
    }
    stage('Run') {
      steps {
        bat 'docker run -d -p 3000:3000 node-app'
      }
    }
  }
}