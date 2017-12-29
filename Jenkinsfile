pipeline {
    agent none
    options { 
		buildDiscarder(logRotator(numToKeepStr: '10')) 
		disableConcurrentBuilds()
		timeout(time: 1, unit: 'HOURS')
    } 
    stages {
        stage('Build Docker Image') {
			agent { label 'python27' }
			steps {
				script {
					sh 'ls'
				}
            }
        }
    }
}