pipeline{
	agent {
		docker { image 'python:0.1'}
	}
	stages {
		stage('Test') {
			steps{
				sh 'curl localhost:8000'
			}
		}
	}
}
