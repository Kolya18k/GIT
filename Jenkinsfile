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