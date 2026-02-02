pipeline {
    agent {
        docker {
            image 'python:3.10-slim'
        }
    }

    stages {

        stage('Python Version') {
            steps {
                sh "python --version"
            }
        }

        stage('Docker Version') {
            steps {
                sh "echo Docker is running on host (Windows)"
            }
        }

        stage('Install Make') {
            steps {
                sh "apt-get update"
                sh "apt-get install -y make"
                sh "make --version"
            }
        }
    }
}
