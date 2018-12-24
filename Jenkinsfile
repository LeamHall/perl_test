pipeline {
    agent { docker { image 'perl' } }
    stages {
        stage('build') {
            steps {
                sh 'perl --version'
                perl Build.PL
                ./Build
                ./Build test
            }
        }
    }
}
