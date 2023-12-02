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
                sh 'docker build -t tde .'
            }
        }
        stage('Composer'){
            steps{
                sh 'docker-compose up'
            }
        }
        stage('Stop Docker Compose') {
            steps {
                script {
                    sh 'docker-compose down'
                    echo 'DEU CERTOOOOOOOOO, ALELUIAAAAAAAAAA!!!!!!!!!!'

                }
            }
        }
    }
}
