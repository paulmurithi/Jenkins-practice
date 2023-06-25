pipeline{
    agent any
    stages{
        stage("Clone"){
            steps{
                sh echo "testing failed message"
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
        success{
            slackSend color:good message: "Build success - ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
        }
        failed{
            slackSend color:danger message: "Build failed - ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
        }
    }
}