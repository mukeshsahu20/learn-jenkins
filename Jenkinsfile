pipeline {
    agent any

    stages {

        stage('Stage 1 - Start') {
            steps {
                echo "Stage 1 is working"
            }
        }

        stage('Stage 2 - Build') {
            steps {
                echo "Building application..."
                sh 'sleep 5'
            }
        }

        stage('Stage 3 - Test') {
            steps {
                echo "Running tests..."
                sh 'sleep 5'
            }
        }

        stage('Stage 4 - Deploy DEV') {
            steps {
                echo "Deploying to DEV..."
                sh 'sleep 5'
            }
        }
    }

    post {
        success {
            echo "All stages executed successfully ✅"
        }
        failure {
            echo "Pipeline failed ❌"
        }
    }
}