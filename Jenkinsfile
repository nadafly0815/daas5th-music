pipeline {
	agent any

	stages {
		stage('Preparation') {
			steps {
			    cleanWs()
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

