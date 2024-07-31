pipeline {
	agent any 	
	stages {
		stage('Checkout') {
			steps {
				echo 'Checkout completed'
				echo 'Checkout is done'

			}
		}
		stage('Static-test') {
			steps {
				echo 'Running static tests on code'
			}
		}
		stage('Build') {
			steps {
				sh 'echo "Building the code"'
			}
		}
		stage('Deploy') {
		    when {
                branch 'prod'
            }
			steps {
				echo 'Deploying into environment'
			}
		}
	}
}
