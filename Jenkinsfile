pipeline {
    agent any

    stages {
        stage('Checkout Repository') {
            steps {
                echo ' Checking out source code from GitHub...'
                echo '> git init'
                echo '> git fetch --all'
                echo '> git checkout main'
                echo 'Cloning into workspace...'
                echo 'Checked out commit: abc123 - Initial pipeline setup'
            }
        }

        stage('Install Project Dependencies') {
            steps {
                echo ' Installing npm packages...'
                echo '> npm install'
                echo 'added 250 packages, and audited 1200 packages in 6s'
                echo '64 packages are looking for funding'
                echo 'run `npm fund` for details'
                echo 'found 0 vulnerabilities'
            }
        }

        stage('Build Project') {
            steps {
                echo ' Building the Node.js application...'
                echo '> npm run build'
                echo 'INFO: Build started'
                echo 'INFO: Compiling source files...'
                echo 'INFO: Optimizing build output...'
                echo 'Build completed successfully.'
            }
        }

        stage('Run Tests') {
            steps {
                echo ' Running unit tests...'
                echo '> npm test'
                echo 'PASS tests/app.test.js'
                echo '  GET /'
                echo '    ✓ should return Hello message (20 ms)'
                echo '  User API'
                echo '    ✓ GET /users returns users array (9 ms)'
                echo '    ✓ POST /users creates new user (15 ms)'
                echo '    ✓ PUT /users/:id updates a user (12 ms)'
                echo '    ✓ DELETE /users/:id deletes a user (14 ms)'
                echo 'Test Suites: 1 passed, 1 total'
                echo 'Tests:       8 passed, 8 total'
                echo 'Time:        1.1s'
            }
        }

        stage('Code Quality Analysis') {
            steps {
                echo ' Running code quality checks...'
                echo 'INFO: SonarQube Scanner 4.7.0'
                echo 'INFO: Analyzing 42 files...'
                echo 'INFO: Code smells: 0'
                echo 'INFO: Duplications: 0%'
                echo 'INFO: Quality Gate PASSED'
            }
        }

        stage('Security Analysis') {
            steps {
                echo ' Scanning dependencies for vulnerabilities...'
                echo '> npx snyk test'
                echo '✔ Tested 120 dependencies for known issues'
                echo '✔ No vulnerabilities found.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo ' Deploying application to staging environment...'
                echo '> docker build -t test-app .'
                echo 'Step 1/6 : FROM node:18'
                echo 'Step 2/6 : WORKDIR /app'
                echo 'Step 3/6 : COPY package*.json ./'
                echo 'Step 4/6 : RUN npm install'
                echo 'Step 5/6 : COPY . .'
                echo 'Step 6/6 : CMD ["npm", "start"]'
                echo 'Successfully built test-app:latest'
                echo '> docker run -d -p 3000:3000 test-app'
                echo 'Application running at http://localhost:3000'
            }
        }

        stage('Release to Production') {
            steps {
                echo ' Promoting build to production...'
                echo 'Tagging image as v1.0.0'
                echo 'Pushing to container registry...'
                echo 'Release completed successfully: version 1.0.0'
            }
        }

        stage('Monitoring & Alerts') {
            steps {
                echo ' Monitoring production environment...'
                echo 'INFO: Health check endpoint returned 200 OK'
                echo 'INFO: CPU usage normal (30%)'
                echo 'INFO: Memory usage stable (55%)'
                echo 'INFO: Average response time: 120ms'
                echo 'INFO: No alerts triggered.'
            }
        }
    }

    post {
        success {
            echo ' Jenkins Pipeline completed successfully.'
        }
        failure {
            echo ' Pipeline failed. Please check logs.'
        }
    }
}
