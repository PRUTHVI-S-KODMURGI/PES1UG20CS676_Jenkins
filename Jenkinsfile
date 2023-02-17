pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C main'
                echo 'successful build!'
            }
        }
        stage('Test') {
            steps {
                sh 'hello_exec'
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
