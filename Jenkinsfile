pipeline {
    agent any

    stages {


         stage('get git tag') {
            steps {
             script {
             latestTag = sh(returnStdout:  true, script: "git tag  | head -n 1").trim()
             env.BUILD_VERSION = latestTag
             echo "env-BUILD_VERSION"
             echo "${env.BUILD_VERSION}"
                }
            }
         }

         stage('Test') {
            steps {
                sh "echo 'dotnet test' "
            }
        }
        stage('dotnet publish') {
            steps {
                sh "echo 'publish'"    
                               
                
            }
        }
    }
}