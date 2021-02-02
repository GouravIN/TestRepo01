@Library('shared-library') _

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
                    command label: 'running sleep', 'sleep 10'
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