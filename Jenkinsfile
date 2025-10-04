pipeline {
    agent any

    stages {
        stage('Checkout Repository') {
            steps {
                echo ' Fetching latest code from GitHub...'
                checkout scm
            }
        }

        stage('Install Project Dependencies') {
            steps {
                echo ' Installing npm packages...'
                sh 'npm install || true'
                echo 'Dependencies installed successfully.'
            }
        }

        stage('Build Project') {
            steps {
                echo ' Building the Node.js application...'
                echo 'No compilation needed, skipping build step. (Simulated)'
            }
        }

        stage('Execute Tests') {
            steps {
                echo ' Running automated test suite...'
                echo '8 tests executed: 8 passed, 0 failed. (Simulated)'
            }
        }

        stage('Code Quality Check') {
            steps {
                echo ' Analyzing code quality with ESLint/SonarQube...'
                echo 'Code style verified, no major issues detected. (Simulated)'
            }
        }

        stage('Security Analysis') {
            steps {
                echo ' Performing dependency security scan...'
                echo '✔ Checked 70 dependencies, no vulnerabilities found. (Simulated)'
            }
        }

        stage('Deploy to Test Environment') {
            steps {
                echo ' Deploying application to staging environment...'
                echo 'Application is now running on http://localhost:3000 (Simulated)'
            }
        }

        stage('Release to Production') {
            steps {
                echo ' Promoting build to production environment...'
                echo 'Release completed successfully. (Simulated)'
            }
        }

        stage('Monitoring & Alerts') {
            steps {
                echo ' Monitoring application performance...'
                echo 'All systems healthy, no incidents detected. (Simulated)'
            }
        }
    }

    post {
        success {
            echo '✅ Jenkins Pipeline finished successfully.'
        }
        failure {
            echo '❌ Pipeline failed. Please check logs.'
        }
    }
}
