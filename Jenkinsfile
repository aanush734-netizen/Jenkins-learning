pipeline {
    agent any

    stages {
        stage ('checkout') {
            steps {
                echo 'checking out code'
                checkout scm
            }
        }
        stage('build') {
            steps {
                echo 'building new sh command'
                sh 'whoami'
                sh 'pwd'
                sh 'docker --version'
            }
        }
    }
}
