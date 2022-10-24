pipeline {
  agent{
    docker { image 'ishmailbari/server:latest'}
  }
  stages {
    stage ('image build and Push') {
      steps {
        sh 'python3 --version'
      }
    }
  }
}
