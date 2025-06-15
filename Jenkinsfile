pipeline {
    
    agent any 
    tools {maven "mavenV3"}
    stages {
        stage ("checkout") {
            steps{
                 git branch :"main" , url :"https://github.com/7oda111/SpringRESTful.git"
            }
           
        }
        stage("buid") {
            steps{
                sh "mvn compile"
            }
        }
        stage("test") {
            steps{
                sh "mvn test"
            }
        }

    }
    
}
    
