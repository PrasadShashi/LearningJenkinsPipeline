pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
                sh 'javac Test.java'
            }
        }
        stage('build') {
            steps {
                sh 'java Test'
            }
        }
    }
}