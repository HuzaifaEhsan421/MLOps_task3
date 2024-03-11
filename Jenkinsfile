// Add jenkins file to checkout , install dependencies and execute test.py file
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                script {
                    checkout scm
                }
            }
        }
        stage('Install dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }
        stage('Execute test.py') {
            steps {
                bat 'python test.py'
            }
        }
    }
}

