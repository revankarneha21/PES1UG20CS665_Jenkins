pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o neha PES1UG20CS665.cpp'
                build job : 'PES1UG20CS665-1'
                echo 'build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './neha1'
                echo 'test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'pipeline failed'
                }
            
        
    }
}
