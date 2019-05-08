pipeline {
	agent any

	stages {
		stage('Preparation') {
			steps {
        deleteDir()
        retry(3) { checkout scm }
			}
		}
		stage ('Delivery') {
			steps {
        echo "Delivery!"
			}
		}
		stage('Deploy') {
			steps {
        echo "Deploy!"
			}
		}
		stage('Cleanup') {
			steps {
        echo "Cleanup!"
      }
		}
	}
}

