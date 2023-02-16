pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'build PES1UG20CS676-1'
            }
        }
        stage('Test') {
            steps {
                sh 'build PES1UG20CS676-2'
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
