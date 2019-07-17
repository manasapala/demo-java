pipeline {
    agent any {
    stages {
          
          stage('Cloning from SCM & cleaning the repo'){
            steps{
              
              git 'https://github.com/manasapala/demo-java.git'
              
              }
          }
          stage('Test'){
            steps{
                
                sh "/usr/lib/apache-maven-3.6.0/bin/mvn test"
                }
               }
          stage('Build & Package'){
            steps{
                
                sh "/usr/lib/apache-maven-3.6.0/bin/mvn package"
                }
               }
          }
   }
   }
