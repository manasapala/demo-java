pipeline {
    agent any {
    stages {
          
          stage('Cloning from SCM & cleaning the repo'){
            steps{
              
              git 'https://github.com/manasapala/demo-java.git'
              
              }
          stage('Test'){
            steps{
                
                sh "mvn test"
                }
               }
          stage('Build & Package'){
            steps{
                
                sh "mvn package"
                }
               }
          }
   }
   }
