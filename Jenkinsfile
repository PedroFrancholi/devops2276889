pipeline{
    
    agent any
    
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
