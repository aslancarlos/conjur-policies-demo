pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'conjur -i policy load -b root -f Users/users.yml'
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
