pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git url: 'https://github.com/yashuchavhan38/portfolio.git'
            }
        }
        stage('Install') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                bat 'npm test'
            }
        }
        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment step - Add your deployment commands'
            }
        }
    }
}
