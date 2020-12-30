pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "dotnet build"
            }
        }
        stage('Test') {
            steps {
                echo 'Stage Test'
            }
        }
        stage('Deploy') {
            steps {
                sh "dotnet publish"
            }
        }
    }
}