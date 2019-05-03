pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('step1') {
            steps {
                echo "un"
            }
        	stages {
	        	stage('step2') {
                		steps {
                    		echo "bonjour BORIS"  
                		}
        		}
        		stage('step3') {
                		steps {
                    		echo "bonjour HENRI" 
                		}
        		}
     		}
		}
	}
}