node {
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