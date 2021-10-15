pipeline {
	agent any
	tools {
        maven 'Maven_3.8.3' 
    }
	stages{
		stage('Compile Stage'){
				
			steps{
                bat "mvn clean compile" 
        	}
		
		}
		stage('Testing Stage'){
			steps{		
				echo 'COmpleted!'
			}		
		}
	}
}
