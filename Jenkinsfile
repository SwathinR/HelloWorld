pipeline {
	agent any
	tools {
        maven 'Maven_3_8_3' 
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
