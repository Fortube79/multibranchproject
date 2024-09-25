pipeline {
    agent any
    environment {
        CI = 'true'
    tools {
        nodejs 'NodeJS' // Usa el nombre que diste a la instalación de NodeJS
    }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
   }
}
