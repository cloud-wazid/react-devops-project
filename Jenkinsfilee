@"
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'React code checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Building React application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing React application...'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t react-devops-app .'
            }
        }

    }
}
"@ | Set-Content Jenkinsfile