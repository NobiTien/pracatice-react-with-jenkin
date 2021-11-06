pipeline {
    agent none
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'node:lts-buster-slim'
                    args '-p 3000:3000'
                }
            }
            environment {
                CI = 'true'
            }
            steps {
                sh 'npm install' 
            }
        }
    }
}