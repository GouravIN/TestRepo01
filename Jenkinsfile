@Library('gourav-shared') _

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