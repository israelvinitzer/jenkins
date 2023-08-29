pipeline {
    agent any

    environment {
        PATH = "/usr/local/bin:${env.PATH}"
    }

    stages {
        stage('Verify Branch') {
            steps {
                sh '''
                   echo "$GIT_BRANCH"
                   whoami
                   cd /Users/ivinitzer/Documents/repo/azure-voting-app-redis
                   docker ps -a
                   docker build -t jenkins-pipeline .
                   docker images -a
                   '''
            }
        }
    }
}
