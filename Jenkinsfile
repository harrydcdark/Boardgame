pipeline {
    agent any
    tools {
        jdk 'JDK17'
        maven 'Maven3'
    }

    stages {
        stage('git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/harrydcdark/Gitboard.git'
            }
        }
        
        stage('maven compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('maven test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('maven package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
