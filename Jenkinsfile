pipeline {
    agent any
   
    stages {
        stage('Sonarqube Check Quality') {
            steps {

                script{
                    withSonarQubeEnv(credentialsId: 'sonar-token') {
                    sh 'chmod +x gradlew'
                    sh './gradlew sonarqube'
                }
                }
                
            }
        }

         

        
    }
}