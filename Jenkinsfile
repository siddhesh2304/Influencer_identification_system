pipeline {
    agent any

    stages {
        stage('Build and Run') {
            steps {
                // Build and run the Docker containers using Docker Compose
                bat 'docker-compose up --build -d'
            }
        }

        stage('Test') {
            steps {
                // Run tests against the running containers
                bat 'docker-compose exec app npm run test'
            }
        }
    }

    post {
        always {
            // Clean up resources, stop and remove the containers
            bat 'docker-compose down'
        }
        success {
            // Actions to perform on successful build
        }
        failure {
            // Actions to perform on build failure
        }
    }
}
