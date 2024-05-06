pipeline {
agent none
stages {
    stage('Build') { 
        agent any
              steps {
              echo "This is Build"
            }
        }
        stage('Test') { 
          agent { label 'Label1' } 
          steps {
               echo "This is Test"
            }
        }
        stage('Deploy') { 
          agent { label 'master' }
            steps {
                echo "This is Deploy"
            }
        }
    }
}
