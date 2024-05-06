Pipeline {
    agent any
        stages {
            agent { label 'Label2'} 
                    steps {
                        echo " This is build"
            }
        }
            stage('Test') {
                agent { label 'Label1'}
                    steps {
                        echo "This is test"
            }
        }
            stage('Deploy') {
                agent { label 'Label2'}
                    steps {
                        echo "This is deploy"
            } 
        }
    }
}
