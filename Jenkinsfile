
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/mounika892/internship-website-two.git'
            }
        }

        stage('Deploy Website Two') {
            steps {
                sh '''
                    sudo install -m 644 index.html /var/www/website-two/index.html
                '''
            }
        }
    }
}
