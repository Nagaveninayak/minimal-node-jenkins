pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                script {
                    docker.image('node:22.20.0-alpine3.22').inside('-v /tmp:/tmp') {
                        sh 'node --version'
                    }
                }
            }
        }
    }
}
