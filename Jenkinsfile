pipeline {
	agent any
	stages {
		steps{
		stage('Compile Stage'){
			withMaven(maven: 'Maven_3_8_3')
				sh 'mvn clean compile'
			}
		}
	}
	
}
