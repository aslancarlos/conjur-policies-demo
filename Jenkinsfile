pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Gitlab-jwt') {
            steps {
                sh 'conjur -i policy load  -b root -f authn/gitlab-jwt.yml'
            }
        }
    }
}
