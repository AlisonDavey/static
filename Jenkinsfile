pipeline {
     agent any
     stages {
          stage('Build') {
              steps {
                  sh 'echo "Hello World"'
                    }
              stage('Lint HTML') {
                   sh 'tidy -q -e *.html'
                    }
         }
     }
}
