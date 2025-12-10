pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                // Install Node.js dependencies
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                // Run your Node.js tests (assuming you have them in package.json)
                sh 'npm test'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}

