pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/yourusername/devops-cicd-project.git'
            }
        }

        stage('Debug Files') {
            steps {
                sh 'pwd'
                sh 'ls -la'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh '/opt/homebrew/bin/docker build -t devops-app .'
            }
        }
    }
}
