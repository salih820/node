pipeline {
    agent any

    stages {
        stage('Backend Install') {
            steps {
                bat 'cd backend && npm install'
            }
        }

        stage('Backend Test') {
            steps {
                bat 'cd backend && npm test'
            }
        }

        stage('Frontend Install') {
            steps {
                bat 'cd frontend && npm install'
            }
        }

        stage('Frontend Build') {
            steps {
                bat 'cd frontend && npm run build'
            }
        }
    }
}