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
                sh "cd /var/lib/jenkins/workspace/myaspcore/bin/Debug/netcoreapp3.1"
                sh "scp -r publish root@94.232.174.159:/tmp"
            }
        }
    }
}