pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ hello.cpp'
                sh 'PES1UG20CS676-1'
            }
        }
        stage('Test') {
            steps {
                sh 'PES1UG20CS676-2'
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
