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
                echo 'dotnet test'
            }
        }
        stage('Deploy') {
            steps {
                sh "dotnet publish"
            }
        }
    }
}