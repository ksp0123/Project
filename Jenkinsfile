pipeline {
    agent any
    tools {
        maven 'maven3'
    }
    stages {
        steps {
        stage('Build Artifact') {
            sh 'mvn clean package'
            } 
        }
      
     stage('Unit test') {
        steps {
       sh 'mvn test'
} 
        }

     stage('integration test') {
       steps {
       sh 'mvn verify -DskipTest'
} 
       }   
}
}