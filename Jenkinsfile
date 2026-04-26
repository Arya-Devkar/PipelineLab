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
post {
    success {
        emailext(
            subject: 'Build Successful',
            body: 'Pipeline executed successfully',
            to: 'aryadevkar403@gmail.com'
        )
    }
    failure {
        emailext(
            subject: 'Build Failed',
            body: 'Pipeline failed',
            to: 'aryadevkar403@gmail.com'
        )
    }
}
