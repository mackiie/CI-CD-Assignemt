pipeline{
    agent any
    stages{
        stage('Clean'){
            steps{
                echo "Clean Stage"
                sh "mvn clean"
            }
        }
        stage('Test'){
            steps{
                echo "Test Stage"
                sh "mvn test"
            }
        }
        stage('Package'){
            steps{
                echo "Package Stage"
                sh "mvn package"
            }
        }
        stage('Deploy'){
            steps{
                echo "Deploy Stage"
                sh "mvn deploy"
            }
        }
    }
}
