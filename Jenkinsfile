pipeline {
    agent any
    stages {
        stage('Upload S3') {
            steps {
                withAWS(region:'us-east-2',credentials:'aws-static')
                sh 'echo "Hello World"'
            }
        }
    }
}
