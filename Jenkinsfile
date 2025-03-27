node {
    docker.image('node:lts-buster-slim').withRun('-p 3001:3001')
    stage('Build') { 
        sh 'npm install'
    }
    stage('Test') {
        sh './jenkins/scripts/test.sh'
    }
}