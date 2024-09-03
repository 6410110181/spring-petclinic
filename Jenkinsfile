#!groovy
pipeline {
    agent none
   stages {     
    stage('Build') {
      agent {         
       docker {          
         image ('anapsix/alpine-java').inside {sh 'java -version'}       
  }
}       
  steps {
       sh 'mvn clean install'
       }
     }
   }
 }