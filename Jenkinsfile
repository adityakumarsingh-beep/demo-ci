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
