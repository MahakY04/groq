
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                checkout scm
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        // Optional deploy stage, commented out since you mentioned no deployment
        // stage('Deploy') {
        //     steps {
        //         // Add deployment steps here
        //     }
        // }
    }
}
