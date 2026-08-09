pipeline {
    agent any

    stages {

             stage('Check Python Environment') {
            steps {
                sh '''
                    python --version
                    pip --version
                    google-chrome --version
                '''
            }
        }
}
 post {
        success {
            echo 'The test passed!'
        }
        failure {
            echo 'The test failed!'
        }

    }
}
