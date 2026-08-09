pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/mrsolankigit/Jenkins_Python_Selenium.git'
            }
        }

        stage('Check Python Environment') {
            steps {
                sh '''
                    python3 --version
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
