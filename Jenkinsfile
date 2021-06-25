pipeline {
    agent none
    stages {
        stage('Back-end') {
            agent {
                docker { 
                    image 'maven:3.8.1-adoptopenjdk-11' 
                    label 'centos8'
                }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
                docker { 
                    image 'node:14-alpine' 
                    label 'centos8'
                }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
