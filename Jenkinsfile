pipeline {
    agent {
        docker {
            image 'node:8-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm --version'
                withDockerContainer(args: "-u root", image: "${JOB_NAME}") {
            sh "npm install"
        }
            }
        }
    }
}

