pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('Initialize'){
            def dockerHome = tool 'myDocker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
        }
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}
