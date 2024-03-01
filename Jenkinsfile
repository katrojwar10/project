pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'build'
                echo 'Building..Building '
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo 'test'
                echo 'Testing..Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo 'Deploy'
                echo 'Deploying.... Testing'
            }
        }
    }
        
     post {
        success {
            mail to: akshaykatrojwar@gmail.com, subject: 'The Pipeline success :('
        }
        failure {
            mail to: katrojwarakshay10@gmail.com, subject: 'The Pipeline failed :('
        }
     }
}
