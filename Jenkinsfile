
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
                echo 'Code downloaded from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Python Project'
                bat 'python --version'
            }
        }

        stage('Test') {
            steps {
                bat 'python app.py'
            }
        }

        stage('Success') {
            steps {
                echo 'Jenkins Build Completed Successfully!'
            }
        }
    }
}
