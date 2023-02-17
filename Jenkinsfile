pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ hello.cpp'
                echo 'successful build!'
            }
        }
        stage('Test') {
            steps {
                sh 'a.exe'
                echo 'successful test!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'success!'
            }
        }
    }
    post {
        failure {
           echo 'failed!'        
        }
    }
}
