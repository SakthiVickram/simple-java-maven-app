pipeline {
    agent any
    tools{
    maven 'maven3.6'
    jdk 'openjdk11'
  }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
                sh 'ls'
                sh 'pwd'
                
            }
        }
       
     
    }
}
