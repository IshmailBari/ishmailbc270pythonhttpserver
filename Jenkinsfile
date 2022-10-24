pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
           docker run --publish 8080:8080 ishmailbari/server:latest
      }
    }
  }
}
