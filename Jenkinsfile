pipeline {
    libraries {
        lib 'gourav-shared@master'
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