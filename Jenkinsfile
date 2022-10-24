pipeline {
    agent any 
    environment {
    DOCKERHUB_CREDENTIALS = credentials('docker-hub-ishmailbari')
    }
    stages {
        stage('Build docker image') {
            steps {  
                sh 'sudo docker build . -t ishmailbari/server:latest .'
            }
        }
        stage('Run docker image') {
            steps {  
                sh 'sudo docker run -p 8000:8000 ishmailbari/server:latest.'
            }
        }
        stage('login to dockerhub') {
            steps{
                sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
            }
        }
        stage('push image') {
            steps{
                sh 'sudo docker push ishmailbari/server:latest'
            }
        }
}
post {
        always {
            sh 'sudo docker logout'
        }
    }
}
