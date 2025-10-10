pipeline {
    agent any
    
    tools {
        maven 'Maven-3.9'
        jdk 'jdk-17'
    }

    stages {
        stage('git checkout') {
            steps {
               git branch: 'main',url: 'https://github.com/devopsbykrishnareddy/Boardgame.git'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
