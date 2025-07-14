
pipeline {
    agent {
        label 'NodeJS_18'
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://your-git-repo-url.com/your-repo-name.git'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                // No deployment command provided, so do nothing
                echo 'No deployment command provided.'
            }
        }
    }
}
