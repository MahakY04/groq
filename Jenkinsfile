Here is a Jenkinsfile for a Node.js project using npm as the build tool:
```
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
```
Let me explain what each part of the Jenkinsfile does:

* `pipeline { ... }`: This defines a Jenkins pipeline.
* `agent any`: This specifies that the pipeline can run on any available agent (e.g., a Jenkins slave).
* `stages { ... }`: This defines the stages of the pipeline.
* `stage('Build') { ... }`: This defines a stage named "Build".
* `steps { ... }`: This defines the steps to be executed in the "Build" stage.
* `checkout scm`: This checks out the source code from the SCM (e.g., Git).
* `sh 'npm install'`: This runs the `npm install` command to install the project dependencies.
* `stage('Test') { ... }`: This defines a stage named "Test".
* `steps { ... }`: This defines the steps to be executed in the "Test" stage.
* `sh 'npm test'`: This runs the `npm test` command to execute the project tests.
* The `Deploy` stage is commented out since you mentioned no deployment is required. If you need to add deployment steps, uncomment this stage and add the necessary steps.

Save this Jenkinsfile in the root of your Node.js project, and Jenkins will automatically detect and execute it when you configure a Jenkins pipeline job.