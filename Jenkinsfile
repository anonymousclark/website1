pipeline {
    agent any 
    stages {
        stage('Building stage') { 
            steps {
                withMaven(maven:'maven 3.8.6'){
                sh 'echo building'
            }
        }
        }
        stage('Testing stage') { 
            steps {
                withMaven(maven:'maven 3.8.6'){
              echo 'testing'
            }
        }
        }
        stage('Deployment Stage') { 
            steps {
               withMaven(maven:'maven 3.8.6'){
              echo 'testing'
            }
        }
        }
        }
        }
