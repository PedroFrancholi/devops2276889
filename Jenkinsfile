pipeline{
    
    agent any

    tools {nodejs 'node'}
    
    stages{
        stage('Preparing'){
          steps{
                sh 'npm install'
             //   // sh 'npm install -g cypress'
                sh 'npm test'
            }
        }
    }
}
