pipeline {
    agent { label 'docker-slave' }

    stage('Checkout') {
	steps {
	    checkout scm
	}
    }

    stages {
        stage('Test') {
            steps {
                sh('tests.sh')
            }
        }
    }
}
