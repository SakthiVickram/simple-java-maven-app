pipeline {
    agent any
    tools{
    maven 'maven3.6'
    
  }
    stages {
        stage('Build') {
            steps {
                sh 'mvn compile test package'
                sh 'ls'
                sh 'pwd'
                
            }
        }
       
     
    }
}
