@Library('shared-library@master') _

pipeline {
    agent any
    parameters {
        choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: '')
        booleanParam(name: 'DEBUG_BUILD', defaultValue: false, description: '')
    }
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