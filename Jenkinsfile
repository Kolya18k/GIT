<<<<<<< HEAD
pipeline {
    agent {
        label 'OneS'
    }
    environment {
        envString = 'true'
    }
    post {
        always {
            bat "echo always"
        }
        failure {
            bat "echo failure"
        }
        success {
            bat "echo success"
        }
    }
    stages {
        stage("Етап") {
            steps {
                bat "echo Повідомлення из Етапа"
                bat "echo Переміщення envString = ${envString}"
                script {
                    scannerHome = tool "sonar-scanner" 
                }
            }
        }
    }
}
=======

>>>>>>> 300722c942d27e82249136537e948757783a14e1
