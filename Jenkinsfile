pipeline {
    agent {
        label 'linux'
    }

    environment {
        PACKAGE_NAME = 'node'
    }

    stages {
        stage('build') {
            steps {
                environment {
                    PROJECT_NAME = 'MINIMAL_NODE_JENKINS'
                }
                echo "PACKAGE NAME is ${PACKAGE_NAME}"
                echo "PACKAGE NAME is ${PROJECT_NAME}"
            }
        }
    }
}