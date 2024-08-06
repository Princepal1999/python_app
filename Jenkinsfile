pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add any build steps here, if necessary
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'python3 -m unittest discover -s tests'
            }
        }
        
        stage('Package') {
            steps {
                echo 'Packaging...'
                // Add any packaging steps here, if necessary
            }
        }
    }
    
    post {
        always {
            echo 'Cleaning up...'
            cleanWs()
        }
    }
}
