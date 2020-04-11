pipeline {
    agent any
    tools{
    maven 'maven3.6'
    
  }
    stages {
        stage('Build') {
            steps {
           
                bat 'mvn compile test package'
                
                
            }
             post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
        stage('SonarQube analysis') {
         steps{
        withSonarQubeEnv(credentialsId: 'sonarqube_token',installationName:'sonarqube') { // You can override the credential to be used
      //sh 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.6.0.1398:sonar'
      bat 'mvn sonar:sonar '
        }
    }
  }
       
     
    }
}
