pipeline{
    
    agent any

    stages{
        stage('Preparing'){
            steps{
                sh 'npm install -g npm@10.2.4'
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