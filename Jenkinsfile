pipeline {
    agent any

    environment {
        APP_NAME = 'myapp'
        ENVIRONMENT = 'development'
        VERSION = '1.0'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'

                echo "Application: ${APP_NAME}"
                echo "Environment: ${ENVIRONMENT}"
                echo "Version: ${VERSION}"

                sh '''
                    echo "Checking application details"
                    echo "App Name: $APP_NAME"
                    echo "Environment: $ENVIRONMENT"
                    echo "Version: $VERSION"
                '''
            }
        }

        stage('Test') {
            steps {
                echo "Testing ${APP_NAME}"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying ${APP_NAME} to ${ENVIRONMENT}"
            }
        }
    }
}
