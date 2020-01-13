pipeline {
    agent { docker { image 'node:6.3' } }
    environment { SECRET = credentials('secreto') }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}
