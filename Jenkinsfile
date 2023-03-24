pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'docker ps -a' 
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
