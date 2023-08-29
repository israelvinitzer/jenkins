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
                   cd /tmp
                   docker ps -a
                   docker build -t jenkins-pipeline .
                   docker images -a
                   '''
            }
        }
    }
}
