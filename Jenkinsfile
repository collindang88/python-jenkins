pipeline {
    agent any 

    stages {
        stage('Prepare') {
            steps {
                echo 'Preparing...'
                sh 'python3 -m venv venv'
                sh '. venv/bin/activate'
                sh 'python3 -m pip install -r requirements.txt --quiet'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'python3 -m unittest'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'echo "Here you would add steps to deploy your application"'
            }
        }
    }
}
