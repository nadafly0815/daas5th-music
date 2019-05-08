pipeline {
	agent any

	stages {
		stage('checkout') {
			steps {
			  echo "checkout!"
        deleteDir()
        retry(3) { checkout scm }
			}
		}
		stage ('install modules') {
			steps {
        echo "Delivery!"
        npm install
			}
		}
		stage('test') {
			steps {
        echo "test!"
        $(npm bin)/ng test --single-run --browsers Chrome_no_sandbox
			}
		}
		stage('Cleanup') {
			steps {
        echo "Cleanup!"
      }
		}
	}
}

