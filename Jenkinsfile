pipeline {
    agent any 
    stages {
        stage('Building stage') { 
            steps {
                echo 'building'
        }
        }
        stage('Testing stage') { 
            steps {
              echo 'tested'
            }
        }
        
        stage('Deployment Stage') { 
            steps {
                sh  'sudo apt-get install apache2'
                sh  'sudo systemctl start apache2'
                sh  'sudo systemctl enable apache2'
                sh  'sudo rm -rvf /var/www/html'
                sh  'sudo rm -rvf /var/www/html/.git'
                sh  'sudo git clone https://github.com/anonymousclark/website1.git /var/www/html'
                sh  'sudo systemctl reload apache2'
            }
        }
    }
}
        
        
