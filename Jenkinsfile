pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Check Robot Framework') {
            steps {
                sh 'robot --version'
            }
        }

        stage('Run Robot Tests') {
            steps {
                sh 'robot tests/Lab8.robot'
            }
        }
    }
}
