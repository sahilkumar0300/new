pipeline {
    agent any

    environment {
                
	EMAIL = 'shail1032005@gmail.com'
                 
}

stages {

	stage('Build') {
	steps{
		echo 'Trigggered from GitHub webhook!'
		}
	}
		stage('Send Email Notification') {
			steps {
			   emailext(
                                subject: "NestJS App Deployed Successfully on EC2!",
				body: "Your Nest JS app is Deployed!",
				to: "${EMAIL}"
				)
			}
		}
	}
