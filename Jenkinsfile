pipeline {
    agent {
        node {

                label 'roboshop'

        }
    }
    options { disableConcurrentBuilds() }
     parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
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