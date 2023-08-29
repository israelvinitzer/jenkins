pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                sh '''
                   echo "$GIT_BRANCH"
                   whoami
                   cd /tmp
                   docker ps -a
                   '''
            }
        }
    }
}
