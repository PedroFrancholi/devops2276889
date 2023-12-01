pipeline{
    
    agent any

    stages{
        stage('Build TADS'){
            steps{
                sh '''
                npm install -g
                npm test
                '''
            }
        }
    }
}