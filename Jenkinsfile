pipeline{
    
    agent any

    stages{
        // stage('Show project path '){
        // steps {
        //         script {
        //             echo "O caminho do projeto é: ${WORKSPACE}"
        //         }
        //     }
        // }
        stage('Preparing'){
          steps{
            dir('/root/.jenkins/workspace/TDE')
                sh 'npm install -g'
             //   // sh 'npm install -g cypress'
                sh 'npm test'
            }
        }
    }
}
