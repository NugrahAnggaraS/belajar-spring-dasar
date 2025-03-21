pipeline {
    agent any
    stages {
        stage('Check Java') {
            steps {
                sh 'java -version'
            }
        }
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NugrahAnggaraS/belajar-spring-dasar.git'
            }
        }

        stage('Print'){
            steps {
                sh 'echo "Cihuy"'
            }
        }
    }
}
