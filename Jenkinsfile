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
                echo 'building new sh commands'
                sh 'whoami'
                sh 'pwd'
                sh 'docker --version'
                sh 'date'
                sh 'ls -al'
                sh 'hostname'
            }
        }
    }
}
