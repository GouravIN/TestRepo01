@Library('shared-library@master') _

def z = new org.foo.Consul()

pipeline {
    agent any
    stages {
        stage("") {
            steps {
                script {
                    printMessage 'Gourav'
                    command 'sleep 60'
                    z.insleep(10)
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