pipeline{
    
    agent any

    stages{
        stage('Preparing'){
            steps{
                sh 'npm install -g n'
                sh 'n latest'
            }
        }
        stage('Build TADS'){
            steps{
                sh '''
                npm install
                npm test
                '''
            }
        }
    }
}