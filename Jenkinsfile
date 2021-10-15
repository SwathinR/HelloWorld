pipeline {
	agent any
	tools {
        maven 'Maven_3_8_3' 
    }
	stages{
		stage('Compile Stage'){
				
			steps{
                sh "mvn clean compile" 
        	}
		
		}
		stage('Testing Stage'){
			steps{		
				def response = httpRequest (consoleLogResponseBody: true,
     			contentType: 'APPLICATION_JSON',
      			httpMode: 'GET',
      			url: "http://dummy.restapiexample.com/api/v1/employees",
      			validResponseCodes: '200')
    			return response
			}		
		}
	}
}
