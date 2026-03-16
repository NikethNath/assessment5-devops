pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/NikethNath/assessment5-devops.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t 2023bcd0056niketh/_2023bcd0056 .'
            }
        }

        stage('Push Image') {
            steps {
                sh 'docker push 2023bcd0056niketh/_2023bcd0056'
            }
        }

    }
}