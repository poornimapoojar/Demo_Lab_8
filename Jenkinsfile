pipeline {
    agent any
    tools {
        maven 'Maven'  // Uses the configured Maven tool in Jenkins
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/poornimapoojar/Demo_Lab_8.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment commands if needed
            }
        }
    }
}
