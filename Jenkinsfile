pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                //sh "dotnet build"
            }
        }
        stage('Test') {
            steps {
                //echo 'dotnet test'
            }
        }
        stage('Deploy') {
            steps {
                //sh "dotnet publish"
                sh "cd /var/lib/jenkins/workspace/myaspcore/bin/Debug/netcoreapp3.1/publish/"
                sh "echo $USER"

            }
        }
    }
}