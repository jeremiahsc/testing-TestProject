pipeline {
    agent {
        docker {
            image 'node:8-alpine'
            args '-p 3000:3000 -u root'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm --version'

            }
        }
    }
}

