pipeline {
    agent any
    stages {
        stage('Upload S3') {
            steps {
                sh 'echo "Hello World"'
                }
            }
        stage('Lint HTML') {
            steps {
                sh 'tidy -q -e *.html'
                }
        }
    }
}
