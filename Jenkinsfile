pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling Java program'
                bat 'javac helloworld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Executing Java program'
                bat 'java helloworld'
            }
        }
    }

    post {
        success {
            echo 'Build Successful!'
        }

        failure {
            echo 'Build Failed!'
        }
    }
}
