pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'conjur -i policy replace -b root -f authn/authn-azure-nube1.yml'
            }
        }
        stage('Azure'){
            steps {
                sh 'conjur -i policy replace -b root -f Azure/policy.yml'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker ps -a'
            }
        }
    }
}
