pipeline {
    agent any
   
    stages {
        stage('Example1') {
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