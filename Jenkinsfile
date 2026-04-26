pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checked from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage executed'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage executed'
            }
        }
    }

    post {
        success {
            echo 'GitHub Pipeline Successful'
        }
        failure {
            echo 'GitHub Pipeline Failed'
        }
    }
}