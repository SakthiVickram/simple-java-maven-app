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
        }
       
     
    }
}
