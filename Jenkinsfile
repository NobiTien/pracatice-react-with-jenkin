pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "yarn"
                sh "yarn build"
            }
        }
        // stage("Deploy") {
        //     steps {
        //         sh "sudo rm -rf /var/www/jenkins-react-app"
        //         sh "sudo cp -r ${WORKSPACE}/build/ /var/www/jenkins-react-app/"
        //     }
        // }
    }
}