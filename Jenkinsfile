pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                sh '''
                   echo "$GIT_BRANCH"
                   whoami
                   cd /tmp
                   /usr/local/bin/docker ps -a
                   '''
            }
        }
    }
}
