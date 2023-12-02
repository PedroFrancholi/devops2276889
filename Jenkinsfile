pipeline{
    
    agent any

    tools {nodejs 'node'}

    stages{
        stage('Preparing'){
          steps{
             //dir('wsl.localhost/Ubuntu/mnt/wslg/distro/root/Projects\NodeGoat')
                sh 'npm install'
             //   // sh 'npm install -g cypress'
                sh 'npm test'
            }
        }
    }
}
