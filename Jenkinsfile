pipeline {
    agent {
        docker {
            image 'maven:3.8.1-adoptopenjdk-11'
            label 'centos8'
            args '-v $HOME/.m2rtc:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B'
            }
        }
    }
}
