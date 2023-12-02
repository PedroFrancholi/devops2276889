pipeline{
    
    agent any

    stages{
        stage('Preparing'){
          steps{
                sh 'npm install -g'
             //   // sh 'npm install -g cypress'
                sh 'npm test:e2e'
            }
        }
    }
}
