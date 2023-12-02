pipeline{
    
    agent any

    tools {nodejs 'node'}

    stages{
        stage('Start NodeGoat'){
          steps{
                sh 'npm install'
            }
        }
        stage('Test NPM'){
            steps{
                sh 'npm test'
            }
        }
        stage('Construindo Docker'){
            steps{
                sh 'docker build -t tde .'
            }
        }
        stage('Testando Docker'){
            steps{
                sh 'npm test'
            }
        }
        stage('Deploy'){
            steps{
                sh 'docker compose up'
            }
        }
    }
}
