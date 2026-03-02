pipeline {
    agent any

    stages {
        stage('Fetch file') {
            steps {
                git 'https://github.com/beatjoy15/session2.git'
            }
        }
         stage('Build') {
            steps {
                echo 'Building Project'
                bat 'javac Demo.java'
            }
        }
         stage('Executing') {
            steps {
                echo 'Executing program'
                bat 'java Demo'
            }
        }
         stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
    post {
        success{
            echo 'Pipeline executed successsfully'
        }
        failure{
            echo 'Pipeline failed'
        }
    }
}
