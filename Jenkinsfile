node {
    agent {
        docker {
            image 'node:lts-buster-slim' 
            args '-p 3001:3001' 
        }
    }
    stage('Build') { 
        sh 'npm install'
    }
    stage('Test') {
        sh './jenkins/scripts/test.sh'
    }
}