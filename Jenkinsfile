pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script{
                sh 'g++ -o PES1UG22CS104-1 new.cpp'
            }
            }
        }
        stage('Test') {
            steps {
                script{
                sh './PES1UG22CS104-1'
            }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed! Please check the logs.'
        }
        success{
            echo 'Pipeline executed successfully!
    }
}
