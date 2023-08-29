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
                   cd /Users/ivinitzer/Documents/repo/azure-voting-app-redis/azure-vote
                   docker ps -a
                   docker build -t .
                   docker images -a
                   '''
            }
        }
    }
}
