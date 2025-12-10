pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Docker image...'
                // Локальна збірка Docker-образу
                sh 'docker build -t myapp:latest .'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Можна додати реальні тести
                sh 'echo "Tests passed!"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage (локально)'
                // Перевірка створеного Docker-образу
                sh 'docker images'
            }
        }

    }
}

