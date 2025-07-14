
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://your-git-repo-url.com/your-repo-name.git'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
}
