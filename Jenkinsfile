pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage ("Build Frontend"){
            agent {
                docker {
                    image 'node:lts-alpine'
                    args '-p 3000:3000 -p 5000:5000'
                }
            }
            steps {
               dir("frontend-freact-js"){
                    sh "npm install"
               } 
            }
        }
    }
}