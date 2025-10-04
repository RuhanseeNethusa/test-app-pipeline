pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '✅ [Build] Installing dependencies...'
                echo 'Build completed successfully. (Simulated)'
            }
        }
        stage('Test') {
            steps {
                echo '✅ [Test] Running unit tests...'
                echo 'All tests passed. (Simulated Jest output)'
            }
        }
        stage('Code Quality') {
            steps {
                echo '✅ [Code Quality] Running ESLint analysis...'
                echo 'No code smells, all rules passed. (Simulated)'
            }
        }
        stage('Security') {
            steps {
                echo '✅ [Security] Running dependency scan...'
                echo 'No vulnerabilities found. (Simulated npm audit)'
            }
        }
        stage('Deploy') {
            steps {
                echo '✅ [Deploy] Deploying to staging server...'
                echo 'Application deployed successfully. (Simulated)'
            }
        }
        stage('Release') {
            steps {
                echo '✅ [Release] Promoting build to production...'
                echo 'Release completed successfully. (Simulated)'
            }
        }
    }
}
