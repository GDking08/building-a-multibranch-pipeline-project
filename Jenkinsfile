pipeline {
    agent any{
        CI = 'true'
    }
    stages{
        stage('build'){
            steps {
                bat 'npm install'
            }
        }
        stage('test'){
            //ensure script is executable and then runh it
            bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "chmod +x ./jenkins/scripts/test.sh && ./jenkins/scripts/test.sh"'
        }
    }
}