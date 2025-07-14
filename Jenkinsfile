Here is a Jenkinsfile for a Node.js project using npm as the build tool:
```
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/your-repo-name.git'
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
            // No deployment command provided, so this stage is empty
        }
    }
}
```
Let me explain what each part of this Jenkinsfile does:

* `pipeline { ... }`: This is the top-level block that defines the pipeline.
* `agent any`: This specifies that the pipeline can run on any available agent (i.e., Jenkins node).
* `stages { ... }`: This block defines the different stages of the pipeline.
* `stage('Checkout') { ... }`: This stage checks out the code from the specified Git repository using the `git` step.
* `stage('Build') { ... }`: This stage runs the `npm install` command to install the project's dependencies.
* `stage('Test') { ... }`: This stage runs the `npm test` command to execute the project's tests.
* `stage('Deploy') { ... }`: This stage is empty because no deployment command was provided. If you wanted to deploy your application, you would add the deployment command(s) here.

Note that you'll need to replace `https://github.com/your-username/your-repo-name.git` with the actual URL of your Git repository.