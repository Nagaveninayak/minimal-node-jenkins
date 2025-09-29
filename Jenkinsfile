pipeline {
    agent any
    stages {
        stage('Lists-show') {
            steps {
                sh 'ls'
            }
        }
    }
     post {
        success {
            mail to: 'nagaveninayakn@gmail.com',
            subject: "Sucess showing the list:  ${currentBuild.fullDisplayName}"
            body: "The pipeline ${currentBuild.fullDisplayName} completed successfully."
        }
    }
}