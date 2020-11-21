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
                bat "mvn test"
            }
        }
        stage('Package'){
            steps{
                echo "Package Stage"
                bat "mvn package"
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
