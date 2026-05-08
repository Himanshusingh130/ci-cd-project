pipeline {
    agent any

    stages {

        stage('Pull Docker Image') {
            steps {
                sh 'docker pull YOUR_DOCKER_USERNAME/app-ci:latest'
            }
        }

        stage('Stop Old Container') {
            steps {
                sh 'docker stop app-container || true'
                sh 'docker rm app-container || true'
            }
        }

        stage('Run New Container') {
            steps {
                sh 'docker run -d -p 3000:3000 --name app-container YOUR_DOCKER_USERNAME/app-ci:latest'
            }
        }
    }
}
