pipeline {
    agent any
    stages {
        stage('Debug') {
            steps {
                sh 'echo "Pipeline Running Successfully"'
            }
        }
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NugrahAnggaraS/belajar-spring-dasar.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
