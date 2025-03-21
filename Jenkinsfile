pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NugrahAnggaraS/belajar-spring-dasar.git'
            }
        }

        stage('Test') {
            steps {
                sh './mvnw test'
            }
        }
        stage('Build') {
            steps {
                sh './mvnw clean package'
            }
        }
    }
}
