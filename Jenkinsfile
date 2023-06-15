pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                echo 'Preparing...'
                bat 'python -m venv venv'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                bat '.\\venv\\Scripts\\python -m pip install pytest'
                bat '.\\venv\\Scripts\\python -m pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
