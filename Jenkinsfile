pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('checkout') {
            steps {
                git credentialsId: '698b8fc8-ca64-47f5-9b93-659da750f1a6', url: 'https://github.com/BorisFyot/devops2019-jenkins.git', branch: 'tp1'
            }
        }
        stage('build') {
            steps {
                sh 'mvn install'
            }
         }       
        stage('test') {
            steps {
                sh 'mvn test'
            }           
        }        
    }
    post {
      	success {
            sh 'mvn deploy -s settings.xml'       	          
      	}
    }
}