pipeline {
    agent any
    
    tools {nodejs "node"}
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
              sh "pwd"
              dir('frontend') {
              sh "pwd"
              sh 'npm install'
              }
            }
        }
        stage('Deploy') {
            steps {
                echo "Deployed to AWS"
            }
        }
    }
}