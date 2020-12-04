@Library('gourav-shared') _

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    print.printNode 'Gourav'
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