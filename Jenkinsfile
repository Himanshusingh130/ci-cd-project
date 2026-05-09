pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Himanshusingh130/ci-cd-project.git'
            }
        }

        stage('Test') {
            steps {
                echo 'Repository cloned successfully'
            }
        }
    }
}
