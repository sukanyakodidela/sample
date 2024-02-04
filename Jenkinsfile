pipeline {
    agent any
        
    stages {
    	stage('Checkout') {
		steps {
			// Checkout code from Git
			checkout scm
		}
	}
										            
	stage('Build') {
		steps {
			// Your build steps go here
			sh 'echo "Building the project"'
		}
	}
	stage('Test') {		
		steps {	
			// Your test steps go here
			sh 'echo "Running tests"'
		}
	}

	stage('Deploy') {
		steps {
			// Your deployment steps go here
			sh 'echo "Deploying the project"'
		}
	}
   }
																													
																								   post {
																							
	success {
		// Actions to perform after a successful build
		echo 'Build successful. Send notifications, etc.'
		}
		failure {																																														            // Actions to perform after a failed build
		    echo 'Build failed. Send notifications, etc.'
               }
	    }
}
