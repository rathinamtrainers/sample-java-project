pipeline {
    agent {
        node 'centos8'
    }
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'gradle:6.7-jdk11'
                    reuseNode true
                }
            }
            steps {
                sh 'gradle --version'
            }
        }
        stage('Test') {
            agent {
                docker {
                    image 'node:14-alpine'
                    reuseNode true
                }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
