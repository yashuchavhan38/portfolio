pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git url: 'https://github.com/yashuchavhan38/portfolio.git', branch: 'main', credentialsId: '13870e3e-4a63-4212-ac71-5b9deee119aa'
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
                echo 'Deploy stage - Add your deploy command here'
            }
        }
    }
}
