pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                echo 'Preparing...'
                sh 'python3 -m venv venv'
                bat '.\\venv\\Scripts\\activate'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'pip install pytest'
                sh 'pytest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
