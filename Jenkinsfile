pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                // Checkout code from GitHub
                git branch: 'main', url: 
            }
        }
        stage('Build Docker Image') {
            steps {
                // Build Docker image
                sh 'docker build -t my-web-app .'
            }
        }
        stage('Run Tests') {
            steps {
                // Run tests (replace with actual test commands)
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the container
                sh 'docker run -d -p 3000:3000 --name my-web-app my-web-app'
            }
        }
    }
}
