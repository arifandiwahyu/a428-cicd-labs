node{
    withDockerContainer(args: '-p 15000:15000', image: 'node:16-buster-slim'){
        stage('Build') {
            sh 'npm install'
        }
        stage('Test') {
            sh './jenkins/scripts/test.sh'
        }
    }
}