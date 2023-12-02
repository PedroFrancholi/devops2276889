pipeline{
    
    agent any

    tools {nodejs 'node'}

    stages{
        stage('Preparing'){
          steps{
                sh 'npm install'
            }
        }
        stage('Testing'){
            steps{
                sh 'npm test'
            }
        }
        stage('Building'){
            steps{
                sh 'docker build -t TDE .'
            }
        }
    }
}
