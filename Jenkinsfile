pipeline {
    agent any

    stages {

        stage('Checkout Source') {
            steps {
                echo "Fetching code from repository"
            }
        }

        stage('Install Dependencies') {
            steps {
                echo "Installing application dependencies"
            }
        }

        stage('Build Artifact') {
            steps {
                echo "Building application artifact"
            }
        }

        stage('Static Code Analysis') {
            steps {
                echo "Running code quality checks"
            }
        }

        stage('Unit Tests') {
            steps {
                echo "Executing unit tests"
            }
        }

        stage('Package Application') {
            steps {
                echo "Packaging application"
            }
        }

        stage('Deploy to DEV') {
            steps {
                echo "Deploying to DEV environment"
            }
        }

        stage('Post Deployment Validation') {
            steps {
                echo "Running smoke tests on DEV"
            }
        }
    }

    post {
        success {
            echo "DEV pipeline completed successfully ✅"
        }
        failure {
            echo "Pipeline failed ❌"
        }
    }
}