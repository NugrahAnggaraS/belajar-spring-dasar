pipeline{
    agent any
    stages{
        stage('Checkout'){
            step{
                git branch: 'main',url: 'https://github.com/NugrahAnggaraS/belajar-spring-dasar.git'
            }
        }  

        stage('Build'){
            step{
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