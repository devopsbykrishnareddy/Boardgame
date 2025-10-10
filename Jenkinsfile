pipeline {
    agent any
    
    tools {
        maven 'Maven-3.9'
        jdk 'jdk-17
    }

    stages {
        stage('git checkout') {
            steps {
               git branch: 'main',url: 'https://github.com/devopswithkrishnareddy/Boardgame.git'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
               sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
