pipeline{
    agent any

    stages{
        stage('Build'){
            steps{
                sh '''
                docker --version
                docker-compose --version
                java --version
                jenkins --version
                '''
            }
        }
    }
}