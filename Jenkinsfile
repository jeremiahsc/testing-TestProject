Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker { image 'node:9.2' } }
    stages {
        stage('build') {
            steps {
                sh 'echo starting build'
                sh 'npm install'
                sh 'echo install complete'
                sh 'npm build'
            }
        }
    }
}
