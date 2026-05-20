pipeline {
    agent {
        node {

                label 'roboshop'

        }
    }
    stages {
        stage('Build') {
            steps {
                script {

                        sh """    
                            echo "Build"
                            exit 1

                        """    
                }
            }
        }
        stage('Test') {
            steps {
                script {

                        sh """    
                            echo "Test"

                        """    
                }
            }
        }
        stage('Deploy') {
            steps {
                 script {

                        sh """    
                            echo "Deploy"

                        """    
                }
            }
        }
    }

     post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {

            echo 'sucess'
        }

        failure {

            echo 'failure'
        }
    }
}