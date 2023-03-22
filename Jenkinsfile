pipeline {
    agent any
   
    stages {
        stage('Example1') {
            steps {
                withSonarQubeEnv(credentialsId: 'sonar-token') {
                sh 'chmod +x gradlew'
                sh './gradlew sonarqube'
            }
            }
        }

         

        
    }
}