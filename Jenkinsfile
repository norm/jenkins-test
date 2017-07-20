pipeline {
    agent { label 'docker-slave' }

    stages {
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
