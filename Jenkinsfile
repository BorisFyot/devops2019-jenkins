pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('step1') {
            steps {
                NAME= input message: 'quel es ton nom ?'
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