pipeline{
    agent any
    tools {
            // Install the Maven version configured as "M3" and add it to the path.
            maven 'maven'
        }
    stages{
        stage("SCM Checkout"){
            steps{
            git 'https://github.com/samben01/KarateWithJenkins.git'
            }
        }
        stage("Maven Build"){
            steps{
                sh '''
                mvn clean install --settings C:\\Users\\giangnt123\\.m2\\settings.xml -DskipTests
                 mv ./application/target/*-SNAPSHOT.jar ./application/target/app.jar
                '''
            }
        }
    }
}