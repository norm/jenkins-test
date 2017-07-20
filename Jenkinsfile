pipeline {
    agent { label 'docker-slave' }

    stages {
	stage('Checkout') {
	    steps {
                sh('mkdir /home/jenkins/workspace')
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
