node {
    checkout scm
    stage('Build') {
                sh '''
		sudo docker version
                sudo docker build -t jogodavelha .
		sudo docker run -i jogodavelha:latest /bin/bash
		java JogoDaVelha
		'''
    }
    stage('Test') {
        echo 'Testing...'
    }
    stage('Deploy') {
        echo 'Deploying...'
    }
}
