pipeline {
    agent any  // Use any agent since we'll manage Docker inside the steps
    stages {
        stage('build') {
            steps {
                script {
                    // Run Node inside a Docker container
                    docker.image('node:22.20.0-alpine3.22').inside('-v /tmp:/tmp') {
                        sh 'echo "Running inside Node container"'
                        sh 'node --version'
                    }
                }
            }
        }
    }
}
