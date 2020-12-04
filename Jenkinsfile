@Library('gourav-shared@master') _

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    printNode 'Gourav'
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