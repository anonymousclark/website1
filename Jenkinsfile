pipeline {
    agent any 
    stages {
        stage('Building stage') { 
            steps {
                sh 'sudo apt-get -y install apache2
                    sudo systemctl start apache2
                    sudo systemctl enable apache2
                    sudo rm -rvf /var/www/html
                    sudo rm -rvf /var/www/html/.git
                    sudo git clone https://github.com/anonymousclark/website1.git /var/www/html'
            
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
        
        
