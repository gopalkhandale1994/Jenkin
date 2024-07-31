pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/gopalkhandale1994/Jenkin.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'

                sh '''
                scp index.html user@192.168.1.8:/var/www/html/
                '''
            }
        }
    }
}