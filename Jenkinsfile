pipeline {
    agent {
        label java
    }
    stages {
        stage('Test') {
            steps {
                docker { image 'node:7-alpine' }
                sh 'node --version'
            }
        }
    }
}
