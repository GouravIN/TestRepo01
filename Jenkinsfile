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
                command label:"Running shell", script: "sleep 10"
            }
            post {
                always {
                    cleanWs()
                }
            }
        }
    }
}