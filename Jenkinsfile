node {
    checkout scm
    stage('Build') {
                sh '''
                docker build -t jogodavelha .
				docker run -i -t jogodavelha:latest /bin/bash
				'''
    }
    stage('Test') {
        echo 'Testing...'
    }
    stage('Deploy') {
        echo 'Deploying...'
    }
}