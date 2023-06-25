pipeline{
    agent any
    stages{
        stage("Clone"){
            steps{
                echo "cloning.."
                git 'https://github.com/paulmurithi/Jenkins-practice.git'
            }
        }
        stage("build"){
            steps{
                echo "building.."
            }
        }
        stage("Test"){
            steps{
                echo "Testing.."
            }
        }
    }
    post{
        always{
            slackSend "Build Started - ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
        }
    }
}