pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build running'
            }
        }
    }

    post {
        success {
            emailext(
                subject: 'Jenkins Build Successful',
                body: 'The Jenkins pipeline executed successfully.',
                to: 'aryadevkar403@gmail.com'
            )
        }

        failure {
<<<<<<< HEAD
            emailext(
                subject: 'Jenkins Build Failed',
                body: 'The Jenkins pipeline failed. Please check console output.',
                to: 'aryadevkar403@gmail.com'
            )
        }
    }
}
=======
            echo 'GitHub Pipeline Failed'
        }
    }
}
>>>>>>> 69e526d (Fix Jenkins pipeline)
