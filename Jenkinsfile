pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Gitlab-jwt') {
            steps {
                sh 'conjur -i policy load  -b apps -f authn/gitlab-jwt.yml'
            }
        }
    }
}
