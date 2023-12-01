pipeline{
    
    agent any

    stages{
        stage('Preparing'){
          steps{
                sh 'npm install -g n'
                sh 'n latest'
                sh 'npm install -g npm@latest'
                sh 'npm install -g cypress'
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}