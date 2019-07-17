pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh "/usr/lib/apache-maven-3.6.0/bin/mvn clean"
            }
        }
        stage('--test--') {
            steps {
                sh "/usr/lib/apache-maven-3.6.0/bin/mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "/usr/lib/apache-maven-3.6.0/bin/mvn package"
            }
        }
    }
}
