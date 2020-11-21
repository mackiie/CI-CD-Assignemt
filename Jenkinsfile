pipeline{
    agent any
    stages{
        stage('Clean'){
            steps{
                echo "Clean Stage"
                bat "mvn -s settings.xml clean"
            }
        }
        stage('Test'){
            steps{
                echo "Test Stage"
                bat "mvn -s settings.xml test"
            }
        }
        stage('Package'){
            steps{
                echo "Package Stage"
                bat "mvn -s settings.xml package"
            }
        }
        stage('Deploy'){
            steps{
                echo "Deploy Stage"
                bat "mvn -s settings.xml deploy"
            }
        }
    }
}
