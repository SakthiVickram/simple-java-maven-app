pipeline {
    agent any
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
