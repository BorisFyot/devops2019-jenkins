pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('exemple') {
        	steps {
                script {
                    def tfHome= tool name: 'Ansible'
                    env.PATH = "/usr/bin/ansible:${env.PATH}"
                    sh 'ansible --version'
                }
            }
    }
}