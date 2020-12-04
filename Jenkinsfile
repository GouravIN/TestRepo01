@Library('shared-library@master') _

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    printMessage 'Gourav'
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