pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                sh '''
                   echo "$GIT_BRANCH"
                   cd /var/tmp
                   docker ps -a
                   '''
            }
        }
    }
}
