pipeline{

    agent any
    environment{
            VERSION_NAME="1.2"
    }
    stages{
        stage("Build"){
            steps{
                bat 'echo "Build Stage"'
                bat 'javac Test.java'
                bat 'echo "${VERSION_NAME}"'
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
    post{
        always{
            bat 'echo "Always"'
        }
        success{
            bat 'echo "Build Success Done"'
        }
        failure{
            bat 'echo "Build Failed"'
        }
    }

}