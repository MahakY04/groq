
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/MahakY04/groq.git'
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
