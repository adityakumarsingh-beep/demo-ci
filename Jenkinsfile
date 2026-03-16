pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-node-app .'
            }
        }

        stage('Tag Docker Image') {
            steps {
                sh 'docker tag devops-node-app adityakumar143/devops-node-app:latest'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker push adityakumar143/devops-node-app:latest'
            }
        }

    }
}
