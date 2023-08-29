pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                sh '''
                   echo "$GIT_BRANCH"
                   cd /tmp
                   docker ps -a
                   '''
            }
        }
    }
}
