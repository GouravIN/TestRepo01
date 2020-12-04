@Library('shared-library@master') _

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    printMessage 'Gourav'
                    command 'sleep 60', label "i'm sleeping for one minute"
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