pipeline {
    agent any
    options {
        buildDiscarder(logRotator(numToKeepStr:'10'))
        ansiColor('xterm')
    }
    stages {
        stage('Build') {
            steps {
		        sh 'echo "Building billing service..."'
       	    }
	    }
	    stage('Build docker image') {
            steps {
                sh 'echo "Building docker image..."'
            }
        }
        stage('Push to docker registry') {
            steps {
                sh 'echo "Pushing docker image..."'
            }
        }
    }
}