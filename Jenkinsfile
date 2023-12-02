pipeline{
    
    agent any

    stages{
        stage('Preparing'){
          steps{
            dir('/Projects/NodeGoat')
                sh 'npm install'
             //   // sh 'npm install -g cypress'
                sh 'npm test'
            }
        }
    }
}
