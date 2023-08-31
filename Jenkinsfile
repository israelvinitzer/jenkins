pipeline {
    agent any

    environment {
        PATH = "/usr/local/bin:${env.PATH}"
    }

    stages {
        stage('Hello World') {
            steps {
                sh '''
                   echo hello world
                   '''
            }
        }
        stage('Run on Master') {
            when { branch 'master2' }
            steps {
                sh '''
                   echo welcome to Master branch
                   '''
            }
        stage('Approve to deploy') {
            steps {
                input message "Deploy?"
            }    
            
        }
    }
}
