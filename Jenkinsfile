pipeline {
    agent any

    stages {
        stage('Fix Git Safety') {
            steps {
                // Эта команда скажет Git не проверять владельца папки
                sh 'git config --global --add safe.directory "*"'
            }
        }
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Read Python File') {
            steps {
                sh 'cat main.py'
            }
        }
    }
}
