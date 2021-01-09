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
                sh "dotnet test "
            }
        }
        stage('Deploy') {
            steps {
                sh "dotnet publish"    
                sh "git tag --sort version:refname"               
                
            }
        }
    }
}