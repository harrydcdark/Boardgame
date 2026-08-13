pipeline {
    agent any
    tools {
        jdk 'JDK17'
        maven 'Maven3'
    }

    stages {
         stage('maven compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('maven test') {
            steps {
                sh 'mvn test' // create unity test / testcases
            }
        }
        stage('maven package') {
            steps {
                sh 'mvn package' // creating build 
            }
        }
    }
}
