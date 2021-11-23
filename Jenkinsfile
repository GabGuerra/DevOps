node {
	agent {
		docker {
		  image 'node:lts-buster-slim'
		  args '-p 8989:8989'
		}
	}
    checkout scm
    stage('Build') {
                sh '''
                sudo docker build -t jogodavelha .
				sudo docker run -i -t jogodavelha:latest /bin/bash
				'''
    }
    stage('Test') {
        echo 'Testing...'
    }
    stage('Deploy') {
        echo 'Deploying...'
    }
}