pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                sh 'echo "Upload to AWS"'
                withAWS(region:'us-east-2',credentials:'aws-static')
            }
        }
    }
}
