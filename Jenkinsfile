pipeline {
    agent any
    tools {
        jdk 'jdk17'
        maven 'mvn3.8'
    }
    stages {

       stage('mvn compile') {
            steps {
                sh 'mvn compile'
            }
        }
       stage('mvn test') {
            steps {
                sh 'mvn test'
            }
        }
       stage('mvn pkg') {
            steps {
                sh 'mvn package'
            }
        }                
    }
}
