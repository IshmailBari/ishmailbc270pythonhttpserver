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
      }
    }
  }
}
