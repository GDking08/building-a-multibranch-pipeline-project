pipeline {
    agent any
    environment {
        CI = 'true' // Setting an environment variable
    }
    stages {
        stage('Build') {
            steps {
                // Run npm install using a batch command
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                // Ensure the script is executable and run it using Git Bash
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "chmod +x ./jenkins/scripts/test.sh && ./jenkins/scripts/test.sh"'
            }
        }
    }
}
