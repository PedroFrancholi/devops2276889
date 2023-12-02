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
            dir('\\wsl.localhost\Ubuntu\mnt\wslg\distro\root\Projects\NodeGoat')
                sh 'sudo npm install'
             //   // sh 'npm install -g cypress'
                // sh 'npm test'
            }
        }
    }
}
