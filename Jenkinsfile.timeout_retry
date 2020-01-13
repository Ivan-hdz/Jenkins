pipeline {
    agent { docker { image 'node:6.3' } }
    environment { SECRET = credentials('secreto') }
    stages {
        stage('build') {
            steps {
		retry(3) { sh 'echo reintenta x3 en caso de error'}
		timeout(time: 3, unit: 'MINUTES') {
			sh 'echo aguanta maximo 3 minutos'
		}
                sh 'echo $SECRET'
            }
        }
    }
}
