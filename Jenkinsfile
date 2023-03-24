pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'conjur -i policy update -b root -f authn/authn-azure-nube1.yml'
            }
        }
        stage('Test'){
            steps {
                sh 'docker ps -a'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker ps -a'
            }
        }
    }
}
