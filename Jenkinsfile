pipeline {
    agent { 
        node {
            label 'docker-minion-alpine'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
              sh'''
              echo "doing some building"
              '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."

              sh'''
              echo "doing some testing in here"
              '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
