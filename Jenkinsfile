pipeline{
    
    agent any

    stages{
        stage('Preparing'){
          steps{
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}