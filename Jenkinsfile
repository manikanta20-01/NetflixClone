pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t netflix-clone .'
                sh 'docker run --rm netflix-clone'
            }
        }
    }
}