pipeline {
    agent any 
    stages {
        stage('Building stage') { 
            steps {
                sh 'sudo apt-get -y install apache2'
                sh  'sudo systemctl start apache2'
                sh   'sudo systemctl enable apache2'
                sh   'sudo rm -rvf /var/www/html'
                sh   'sudo rm -rvf /var/www/html/.git'
                sh   'sudo git clone https://github.com/anonymousclark/website1.git /var/www/html'
            
        }
        }
        stage('Testing stage') { 
            steps {
              echo 'testing'
            }
        }
        
        stage('Deployment Stage') { 
            steps {
              echo 'testing'
            }
        }
    }
}
        
        
