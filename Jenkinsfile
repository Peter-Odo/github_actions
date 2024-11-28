pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }
          stage('Lint the project') {
            steps {
                bat 'npm lint'
            }
        }
          stage('Generate a production build') {
            steps {
                bat 'npm build'
            }
        }
          stage('Run tests') {
            steps {
                bat 'npm test'
            }
        }
          stage('Deploy to GCP') {
            steps {
                echo 'Deploying to GCP.......'
            }
        }
          stage('Application Deployed') {
            steps {
                echo 'Deployment Successful!!!!!'
            }
        }
        
    }
}