pipeline{
    agent any
    tools {
            // Install the Maven version configured as "M3" and add it to the path.
            maven 'Maven'
        }
    stages{
        stage("SCM Checkout"){
            steps{
            git 'https://github.com/Giangtqvn01/my-app'
            }
        }
        stage("Maven Build"){
            steps{
                sh '''
                mvn clean package
                '''
            }
        }
    }
}