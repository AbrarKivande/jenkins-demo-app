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
                sh 'echo "No tests yet"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Starting app...'
                sh 'npm start &'
            }
        }
    }
}
