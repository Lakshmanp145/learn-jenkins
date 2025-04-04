pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        timeout(time: 10, unit: 'SECONDS')
        disableConcurrentBuilds()
        retry(1)
    }
    stages {
        stage('Build') {
            steps {
                
                  sh 'echo "This is Build"'
                  //sh 'sleep 10'

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
                  error 'pipeline failed'
            }
        }
    }
    post { 
        always { 
            echo 'This session runs always'
            deleteDir()
        }
        success { 
            echo 'This session runs when pipeline success'
        }
        failure { 
            echo 'This session runs when pipeline failure'
        }
    }
}

