pipeline {
  agent none
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