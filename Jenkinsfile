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
        }
        stage('step2') {
        	when {
            	NAME "BORIS"
            }
                steps {
                    echo "bonjour BORIS"  
                }
        }
        stage('step2') {
        	when {
            	NAME "HENRI"
            }
                steps {
                    echo "bonjour HENRI" 
                }
        }
	}
}