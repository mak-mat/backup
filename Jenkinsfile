
pipeline {
    agent any
    


    stages {
        stage('git checkout') {
            
            environment {
        key1 = "val2"
            }
            steps {
                sh '''
                pwd
                cal
                date
                ls
            
                '''
              sh 'echo "${key1}"'   
            }
        }
        stage('Build Code') {
            steps {
                echo 'Building the code'
                sh 'ls'
                
                
            }
        }
        stage('Deploy to Test') {
            steps {
                echo 'Deploying in the test Env'
                echo 'this is a test job'
               
            }
        }
        
        stage('Pushing') {
            steps {
                echo 'Pushing the Artifacts on Nexus'
                 sh 'echo "${BUILD_NUMBER}"'
            }
        }
    }
}
