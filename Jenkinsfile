pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
        docker.withServer('tcp://ishmailb.eg.com:8000', 'swarm-certs') {
          docker.image('ishmailbari/server:latest').withRun('-p 8000:8000')
        }
      }
    }
  }
}
