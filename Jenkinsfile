pipeline {
    agent { label 'docker-slave' }

    stages {
        stage('mkdir') {
	    steps {
                sh('mkdir /home/jenkins/workspace')
	    }
        }

	stage('Checkout') {
	    steps {
		checkout scm
	    }
	}

        stage('Test') {
            steps {
                sh('tests.sh')
            }
        }
    }
}
