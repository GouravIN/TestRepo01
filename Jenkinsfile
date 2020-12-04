@Library('shared-library') _

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    printMessage.printNode 'Gourav'
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