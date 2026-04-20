pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Скачиваем код из GitHub...'
                checkout scm
            }
        }
        stage('Read Python File') {
            steps {
                echo 'Проверяем содержимое файла main.py:'
                sh 'cat main.py'
            }
        }
    }
}
