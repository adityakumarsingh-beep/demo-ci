pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/adityakumarsingh-beep/devops-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t adityakumar143/devops-node-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker push adityakumar143/devops-node-app'
            }
        }

    }
}
