pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello, world!"'
                sh '''
                   echo "Multiline shell steps"
                   ls -lah
                   '''
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Testing"'
            }
        }
            
        stage('Deploy') {
            steps {
                sh 'echo "Deploy"'
            }
        }
            
    }
}