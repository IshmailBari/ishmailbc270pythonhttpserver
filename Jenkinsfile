pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
           docker run -p 8080:8080 ishmailbari/server:latest
      }
    }
  }
}
