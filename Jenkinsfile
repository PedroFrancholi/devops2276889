pipeline{
    
    agent any

    tools {nodejs 'node'}
    
    stages{
        stage('Preparing'){
          steps{
                sh 'npm install -g'
             //   // sh 'npm install -g cypress'
                sh 'npm test'
            }
        }
    }
}
