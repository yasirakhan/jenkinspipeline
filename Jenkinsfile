pipeline{

    agent any
    stages{
        stage("Build"){
            steps{
                bat 'echo "Build Stage"'
                bat 'javac Test.java'
            }
        }
        stage("Test"){
            steps{
                bat 'echo "Testing Stage"'
                bat 'echo "stage2"'
            }
        }
        stage("Deploy"){
            steps{
                bat 'echo "Deployment Stage"'
                bat 'java Test.java'
            }
        }
    }

}