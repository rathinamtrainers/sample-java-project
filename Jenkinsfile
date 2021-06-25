pipeline {
  agent {
    docker 'centos:8'
    label 'centos8'
  }
  stages {
    stage('Build') {
      steps {
        sh 'echo "Building"'
      }
    }

    stage('Testing') {
      agent any
      steps {
        sh 'echo "Testing completed"'
      }
    }

  }
}
