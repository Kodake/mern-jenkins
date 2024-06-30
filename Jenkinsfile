pipeline {
    agent any

    stages {
        stage('docker compose down') {
            steps {
                script {
                    bat "docker-compose down"
                }
            }
        }
        stage('docker compose build') {
            steps {
                script {
                    bat "docker-compose build --no-cache"
                }
            }
        }
        stage('docker compose up') {
            steps {
                script {
                    bat "docker-compose up"
                }
            }
        }
    }
}
