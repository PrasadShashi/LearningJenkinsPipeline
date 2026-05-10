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

    post{
        always {
            sh 'echo "This will always run"'
        }
        success {
            sh 'echo "This build is successfull"'
        }
        failure {
            sh 'echo "Fail to build the pipeline"'
        }
    }
}