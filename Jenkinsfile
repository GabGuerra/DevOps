node {
    checkout scm
    stage('Build') {
                sh '''
		echo 'Building java classes..'
		javac ./JogoDaVelha/*.java
		sudo docker version
                sudo docker build -t jogodavelha .
		sudo docker run -t jogodavelha:latest /bin/bash |  java ./JogoDaVelha/JogoDaVelha
		'''
    }
    stage('Test') {
        echo 'Testing...'
    }
    stage('Deploy') {
        echo 'Deploying...'
    }
}
