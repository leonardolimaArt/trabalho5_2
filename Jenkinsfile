pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t olaunicamp .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run --rm olaunicamp'
                }
            }
        }
    }
}