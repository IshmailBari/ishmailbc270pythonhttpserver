pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
           docker build . -t server
           docker run -d -p 8000 server
      }
    }
  }
}
