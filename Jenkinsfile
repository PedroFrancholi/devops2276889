pipeline {
    agent any

    stages {
        stage('Instalar dependências') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Executar testes') {
            steps {
                script {
                    sh 'npm test'
                }
            }
        }

        stage('Construir Docker') {
            steps {
                script {
                    sh 'docker build -t TDE .'
                }
            }
        }

        stage('Iniciar Docker Compose') {
            steps {
                script {
                    sh 'docker-compose up -d'
                }
            }
        }
    }

    post {
        always {
            echo 'Successfull executing!'
        }
    }
}