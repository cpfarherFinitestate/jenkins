/* Requires the Docker Pipeline plugin */
pipeline {
    /*agent { docker { image 'python:3.12.1-alpine3.19' } }*/
    agent any
    stages {
        stage('checkout') {
            steps {
                git branch:'main', url: 'https://github.dev/cpfarher/jenkins'
            }
        }
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
