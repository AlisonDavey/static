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
                sh 'echo "Uploading content with AWS creds"'
                withAWS(region:'ap-southeast-2',credentials:'aws-static')
                s3Upload(file:'index.html', bucket:'alijenkinsudacity', path: 'index.html')
            }
        }
    }
}
