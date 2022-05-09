pipeline {
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Start') {
            steps {
                sh 'gatsby build'
            }
        }
        stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}
