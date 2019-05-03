pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('parallel1') {
        	parallel {
        		stage('etape1.1') {
		            steps {
    		            echo "un"
        		    }
        		}
        		stage('etape1.2') {
		            steps {
    		     	   echo "deux"
        		    }
        		}
        	}
        }
        stage('parallel2') {
        	parallel {
        		stage('etape2.1') {
		            steps {
    		            echo "2 un"
        		    }
        		}
        		stage('etape2.2') {
		            steps {
    		     	   echo "2 deux"
        		    }
        		}
        	}
        }
    }
}