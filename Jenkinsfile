pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Installing dependencies...'
                sh 'npm install'
            }
        }
        stage('Test') {
    steps {
        echo 'Running tests...'
        sh 'npm test || true'
    }
}

            
        
        stage('Code Quality') {
            steps {
                echo 'Running ESLint check...'
                sh 'npx eslint . || true'
            }
        }
        stage('Security') {
            steps {
                echo 'Running security audit...'
                sh 'npm audit || true'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Building Docker image and running container...'
                sh 'docker build -t test-app .'
                sh 'docker run -d -p 3000:3000 test-app'
            }
        }
    }
}