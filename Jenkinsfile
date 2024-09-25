pipeline {
    agent any
    tools {
        nodejs 'NodeJS' // Usa el nombre que diste a la instalación de NodeJS
    }
    environment {
        CI = 'true'
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
