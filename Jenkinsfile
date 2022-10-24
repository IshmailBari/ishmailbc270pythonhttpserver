pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
           docker run -p 8000:8000 ishmailbari/server:latest
      }
    }
  }
}
