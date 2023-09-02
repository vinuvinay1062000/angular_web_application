pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from Git
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Run npm install to install project dependencies
                sh 'npm install'

                // Build the Angular application for production
                sh 'ng build --prod'
            }
        }
        // Add more stages for testing, deployment, etc., as needed
    }

    post {
        success {
            // Define post-build actions, if needed
        }
    }
}

