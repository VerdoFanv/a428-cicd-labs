node {
    docker.image('node:lts-buster-slim').inside('-p 3001:3001') {
        stage('Build') {
            checkout scm
            sh 'npm install'
        }
    }
    // stage('Test') {
    //     sh './jenkins/scripts/test.sh'
    // }
}   