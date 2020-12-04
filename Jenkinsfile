pipeline {
    libraries {
        lib 'shared-libraries@master'
    }
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