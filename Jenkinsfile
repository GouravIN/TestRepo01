@Library('shared-library@master') _

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    printMessage 'Gourav'
                    command 'sleep 60'
                }
            }
            post {
                always {
                    cleanWs()
                }
            }
        }
    }
}