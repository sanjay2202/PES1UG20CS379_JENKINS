pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o pes1ug20cs379_task5 pes1ug20cs379_task5.cpp'
                build job: 'PES1UG20CS379-1'
            }
        }
        
        stage('Test') {
            steps {
                sh './pes1ug20cs379_task5'
            }
        }
        
        stage('Deploy') {
            steps {
                eco 'Deployment Successfulllllllll....'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
