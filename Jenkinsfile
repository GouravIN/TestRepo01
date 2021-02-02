@Library('shared-library@master') _

pipeline {
    agent any
    parameters {
        choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: '')
        booleanParam(name: 'DEBUG_BUILD', defaultValue: false, description: '')
    }
    stages {
        stage("Test") {
            steps {
                script {
                    printMessage 'Gourav'
                    command 'sleep 60'
                    if(DEBUG_BUILD){
                        echo "Its a Debug build"
                    } else {
                        echo "Its not a debug build"
                    }
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