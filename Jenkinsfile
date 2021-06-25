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
      steps {
        sh 'echo "Testing completed"'
      }
    }

  }
}
