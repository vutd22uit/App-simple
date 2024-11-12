pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/vutd22uit/App-simple.git'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'nohup node app.js &'
            }
        }
    }
}
