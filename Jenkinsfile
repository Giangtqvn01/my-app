node{
    agent any
    tools {
            // Install the Maven version configured as "M3" and add it to the path.
            maven 'maven'
        }
    stage('SCM checkout'){
        git 'https://github.com/Giangtqvn01/my-app'
    }
    stage('Compile-package'){
        sh 'mvn package'
    }
}