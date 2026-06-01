pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/rajvbiw/day-2-jenkins-tic-tac-toe.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}