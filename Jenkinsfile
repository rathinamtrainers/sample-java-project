pipeline {
    agent {
        docker { 
            image 'node:14-alpine' 
            label 'centos8'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
