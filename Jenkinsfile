pipeline {
    agent any

    stages {
        stage('fetch code') {
            steps {
                git branch: 'main', url: 'https://github.com/Danielkevin25/pipeline.git'
            }
}
        stage('installing apache') {
            steps {
                sh 'sudo apt install apache2 -y'
            }
}
        stage('deploying the code') {
            steps {
                sh 'sudo cp -R * /var/www/html/'
            }
        }
    }
}
