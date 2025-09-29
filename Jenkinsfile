pipeline {
    agent { docker { image 'node:22.20.0-alpine3.22' } }
    stages {
        stage('build') {
            steps {
                echo 'Checking Node version'
                sh 'node --version'
            }
        }
    }
}