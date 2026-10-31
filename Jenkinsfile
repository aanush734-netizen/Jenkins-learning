pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh 'echo "Application build completed"'
            }
        }

        stage('Test') {
            steps {
                script {
                    def result = sh(
                        script: 'exit 1',
                        returnStatus: true
                    )

                    echo "Test command exit code: ${result}"

                    if (result != 0) {
                        echo 'Test failed, but pipeline will continue'
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage is running'
            }
        }
    }
}
