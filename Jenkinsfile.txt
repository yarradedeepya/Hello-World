pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/yarradedeepya/Hello-World.git'
                }
            }
        stage('Test'){
            steps{
                println "intest"
            
            }
            
        }
        stage('Deploy'){
            steps{
            println "deployed"
            }
        }
    }
    
}    
