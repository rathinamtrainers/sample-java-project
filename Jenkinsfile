node('worker-1') {
    checkout scm
    def customImage = docker.build("my-image:${env.BUILD_ID}")
}
