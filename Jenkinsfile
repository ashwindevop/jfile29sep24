pipeline {
    agent any
    
    stages {
        stage('build') {
            steps {
                sh ' sudo yum remove httpd -y '
                sh ' sudo rm -rf /var/www/html'
                sh ' sudo yum install httpd -y '
                sh ' sudo systemctl start httpd '
                sh ' sudo git clone https://github.com/ashwindevop/myweb1may.git  /var/www/html'
            }
        }
    }
}
