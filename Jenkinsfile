pipeline {
    agent any
    stages {
        stage("Clean Up"){
            steps{
                deleteDir()
            }
        }
        stage("Build"){
            steps{
                    sh "mvn clean install"    
            }
        }
        stage("Test"){
            steps{
                    sh "mvn test"   
            }
        }
        stage("CI"){
            steps{
                echo "CI has been completed"
            }
        }
    }
}
