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
                sh "rm -fr /tmp/publish/*"
                sh "cd /var/lib/jenkins/workspace/myaspcore/bin/Debug/netcoreapp3.1"
                sh "cp -R publish/* /tmp/publish"
            }
        }
    }
}