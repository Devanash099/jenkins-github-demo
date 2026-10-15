pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code is ready in the workspace'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo Build completed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Running basic verification...'
                sh 'test -f Jenkinsfile'
            }
        }
    }

    post {
        success {
            echo 'BUILD SUCCESSFUL!'
        }
        failure {
            echo 'BUILD FAILED!'
        }
    }
}
