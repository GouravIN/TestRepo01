@Library('gourav-shared') _

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
                    if(params.DEBUG_BUILD == true){
                        echo "Its a Debug build"
                    } else {
                        echo "Its not a debug build"
                    }
                     command label:"Running Script", script: "sleep 10"
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