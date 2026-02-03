pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Show branch info new ') {
            steps {
                sh '''
                    echo "BRANCH_NAME: $BRANCH_NAME"
                    git branch
                    git rev-parse --abbrev-ref HEAD
                '''
            }
        }
       



        stage('Build') {
            steps {
                echo "Building branch: ${env.BRANCH_NAME}"
            }
        }
    }
}
