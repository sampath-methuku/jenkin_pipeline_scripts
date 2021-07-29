pipeline {
	agent any
	stages {
   		stage ('Deploy'){
       		parallel {
           		stage('Deploy-Unix') {
           		    	steps {
						echo 'Deploying to Unix'
                	}
            	}
           		stage('Deploy-Windows') {
                	steps {
						echo 'Deploying to Windows'
                 	}
            	}
            	stage('Deploy-Mac') {
                 	steps {
        				echo 'Deploying to Mac'
                 	}
            	}
        	}
        }
		stage ('Test'){
       		parallel {
           		stage('Test-Unix') {
                	steps {
						echo 'Testing to Unix'
                	}
            	}
           		stage('Test-Windows') {
                	steps {
						echo 'Testing to Windows'
                 	}
            	}
            	stage('Test-Mac') {
                 	steps {
        				echo 'Testing to Mac'
                 	}
            	}
        	} 
        }    
   
	} 
}
