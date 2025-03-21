pipeline{
    agent any
    stages{
        stage('test'){
            step{
                sh "./mvnw test"
            }
        }

        stage('build'){
            step{
                sh "./mvnw compile"
            }
            step{
                sh "./mvnw test-compile"
            }
        }
    }
}