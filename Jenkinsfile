pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
            }
	stage('Performance Test') {
            steps {
                echo 'Running JMeter script...'
            }
        }
    }
}