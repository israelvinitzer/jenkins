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
                   cd /tmp/azure-voting-app-redis/azure-vote
                   ls
                   docker ps -a
                   docker build -t jenkins-pipeline .
                   docker images -a
                   '''
            }
        }
    }
}
