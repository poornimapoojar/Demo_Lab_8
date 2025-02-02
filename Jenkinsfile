pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'  // Uses the configured Maven tool in Jenkins
    }
    stages {
        
        stage('Build Artifact') {
            steps {
                sh 'mvn clean package -DskipTests=true'
                archive 'target/*.jar'
            }
        }
       
       
    }
}
