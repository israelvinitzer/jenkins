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
                   docker ps -a
                   docker build -t jenkins-pipeline /Users/ivinitzer/Documents/repo/azure-voting-app-redis
                   docker images -a
                   '''
            }
        }
    }
}
