pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/mohibul361/DepOpsAssignment2.git', 
                branch: 'main',
                credentialsId: 'jenkins_connected'
            }
        }
        
        stage('Verify Checkout') {
            steps {
                bat 'echo Listing files from repository...'
                bat 'dir' 
            }
        }
        
        stage('Read and Output Content') {
            steps {
                bat 'echo Reading hello.txt content:'
                bat 'type hello.txt' 
            }
        }

        stage('Build') {
            steps {
                echo 'Running build...'
                
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                
            }
        }
    }
}