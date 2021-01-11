pipeline {
    agent any

    stages {


         stage('get git tag') {
            steps {
             sh "echo changes to alpha branch"
            }
         }

         stage('Test') {
            steps {
                sh "echo  'dotnet test' "
            }
        }
        stage('dotnet publish') {
            steps {
                sh "echo  'publish'"    
                               
                
            }
        }
    }
}
