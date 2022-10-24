pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
        docker.image('ishmailbari/server:latest').withRun('-p 8000:8000')
      }
    }
  }
}
