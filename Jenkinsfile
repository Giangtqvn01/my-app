pipeline{
    agent any
    tools{
        maven 'Maven'
    }
    stages{
        stage("SCM Checkout"){
            steps{
            git 'https://github.com/samben01/KarateWithJenkins.git'
            }
        }
        stage("Maven Build"){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}