pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the NetflixClone project...'
            }
        }
        stage('test') {
            when {
                expression {
                    BRANCH_NAME == 'main'
                }
            }
            steps {
                echo 'Test the application...'
            }
        }
        stage('deploy') {
             when {
                expression {
                    BRANCH_NAME == 'main'
                }
            }
            steps {
                echo 'Deploy the application...'
            }
        }
    }   
}

