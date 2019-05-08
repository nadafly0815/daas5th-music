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
			}
		}
		stage('Cleanup') {
			steps {
        echo "Cleanup!"
      }
		}
	}
}

