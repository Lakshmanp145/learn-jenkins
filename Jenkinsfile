pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                
                  sh 'echo "This is Build"'

            }
        }
        stage('Test') {
            steps {
                
                  sh 'echo "This id Test"'
                
            }
        }
        stage('Deploy') {
            steps {
                
                  sh 'echo "This is Deploy"'
                
            }
        }
    }
    post { 
        always { 
            echo 'This session runs always'
        }
        success { 
            echo 'This session runs when pipeline success'
        }
        failure { 
            echo 'This session runs when pipeline failure'
        }
}

