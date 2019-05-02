pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'hello world')
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    tools {
        maven 'maven'
    }
    options {
        timeout(time: 1, unit: 'SECONDS')
    }
    environment { 
        PRENOM = 'boris'
        }
    stages {
        stage ('Stage 1') {
            options {
                retry(2)
            }
            steps {
                echo "hello world"
                echo prenom2
                sh 'mvn -v'
            }
        environment { 
            prenom2 = 'henri'
            }
        post {
            failure {
                echo "errrorrr"
            }
        }
        }
        stage ('Stage 2') {
            steps {
                echo "comment vas tu"
                echo prenom3
            }
            environment { 
            prenom3 = 'tony'
            }
        }
        stage ('Stage 3') {
            steps {
                echo "bien et toi?"
                echo PRENOM
                echo "Password: ${params.PASSWORD}"
            }
        }
    } 

}