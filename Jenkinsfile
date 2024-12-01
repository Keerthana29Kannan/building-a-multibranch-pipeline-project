pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                // Use double backslashes to escape backslashes in the path
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c ".\\jenkins\\scripts\\test.sh"'
            }
        }
    }
}
