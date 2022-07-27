pipeline {
    agent any 
    stages {
        stage('Building stage') { 
            steps {
                //
            
        }
        }
        stage('Testing stage') { 
            steps {
              //
            }
        }
        
        stage('Deployment Stage') { 
            steps {
                sh  'sudo systemctl start apache2'
                1
                sh  'sudo systemctl enable apache2'
                sh  'sudo rm -rvf /var/www/html'
                sh  'sudo rm -rvf /var/www/html/.git'
                sh  'sudo git clone https://github.com/anonymousclark/website1.git /var/www/html'
                sh  'sudo systemctl reload apache2'
            }
        }
    }
}
        
        
