node('worker-1') {
    /* Requires the Docker Pipeline plugin to be installed */

    stage('Back-end') {
        docker.image('maven:3.8.1-adoptopenjdk-11').inside {
            sh 'mvn --version'
        }
    }

    stage('Front-end') {
        docker.image('node:14-alpine').inside {
            sh 'node --version'
        }
    }
}
