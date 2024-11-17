 pipeline {
    agent none
    stages {
        stage('Example Build') {
            agent { docker 'node:20' }
            steps {
                echo 'Hello, Node'
                sh 'npm install'
            }
        }
        stage('Example Test') {
            agent { docker 'node:20' }
            steps {
                echo 'Hello, Test'
                sh 'npm test'
            }
        }
    }
}