pipeline {
    agent any

    stages {
        stage('Build and Run') {
            steps {
                // Build and run the Docker containers using Docker Compose
                bat 'docker-compose up --build -d'
            }
        }

        stage('Manual Check') {
            steps {
                // Pause the pipeline and wait for manual approval
                input message: 'Please check if the build is running correctly. Click "Proceed" to continue.',
                      submitterParameter: 'CONTINUE_PIPELINE'
            }
        }
    }

    post {
        always {
            // Clean up resources, stop and remove the containers
            bat 'docker-compose down'
        }
    }
}
