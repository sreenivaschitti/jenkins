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
}