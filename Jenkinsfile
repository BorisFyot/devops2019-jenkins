pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('step1') {
            steps {
                NAME= input message: 'quel es ton nom ?',
            }
        stages {
	        stage('step2') {
    	    	when {
        	    	NAME "BORIS"
           		}
                	steps {
                    	echo "bonjour BORIS"  
                	}
        	}
        	stage('step3') {
        		when {
            		NAME "HENRI"
            	}
                	steps {
                    	echo "bonjour HENRI" 
                	}
        	}
     	}
	}
}