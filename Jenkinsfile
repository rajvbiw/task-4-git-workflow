pipeline {
    agent any

    stages {

        stage('Clean Workspace') {
            steps {
                deleteDir()
            }
        }

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building Docker image'
                sh 'docker build -t internship-task-app .'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
                sh 'echo "No tests defined"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying container'

                sh '''
                    docker stop internship-container || true
                    docker rm internship-container || true
                '''

                sh '''
                    docker run -d \
                    -p 3000:3000 \
                    --name internship-container \
                    internship-task-app
                '''
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished'
        }
    }
}