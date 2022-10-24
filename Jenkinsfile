pipeline {
  agent any
  stages {
    stage ('Build') {
           agent {
             docker {
               image 'ishmailbari/server:latest'
               reuseNode true
             }
           }
      steps {
        sh 'docker run -p 8000:8000 ishmailbari/server'
      }
    }
  }
}
