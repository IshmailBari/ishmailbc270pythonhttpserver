pipeline {
  agent any
  stages {
    stage ('image build and Push') {
      steps {
        sh '''
            ssh to your server with IP # I don't know how you ssh to your server just add that command here
            docker build -t server .
            docker push server
            docker run -d -p 8000:8000 server
        '''
      }
    }
  }
}
