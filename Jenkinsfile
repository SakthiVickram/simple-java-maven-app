pipeline {
    agent any
    tools{
    maven 'maven3.6'
    
  }
    stages {
        stage('Build') {
            steps {
                sh 'ls'
                sh 'pwd'
                sh 'mvn compile test package'
                
                
            }
        }
       
     
    }
}
