pipeline {
    agent { docker { image 'node:6.3' } }
    enviroment { SECRET = credentials('secreto') }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}
