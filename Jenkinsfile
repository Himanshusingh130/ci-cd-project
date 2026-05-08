pipeline {
    agent any

    stages {

        stage('Pull Docker Image') {
            steps {
                sh 'docker pull himanshu1306/app-ci:latest'
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
                sh 'docker run -d -p 3000:3000 --name app-container himanshu1306/app-ci:latest'
            }
        }
    }
}
