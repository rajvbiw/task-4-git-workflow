pipeline {
    agent any

    stages {

        stage('Build') {
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

                sh 'docker stop internship-container || true'
                sh 'docker rm internship-container || true'

                sh '''
                docker run -d \
                -p 3000:3000 \
                --name internship-container \
                internship-task-app
                '''
            }
        }
    }
}