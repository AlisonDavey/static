pipeline {
    agent any
    stages {
        stage('Lint HTML') {
            steps {
                sh 'tidy -q -e *.html'
            }
        }
        stage('Upload S3') {
            steps {
                withAWS(region:'us-east-2',credentials:'aws-static')
            }
        }
    }
}
