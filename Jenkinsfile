pipeline {
    agent { 
        dockerfile {
            filename 'Dockerfile2'
            label 'centos8'            
        }        
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'svn --version'
            }
        }
    }
}
