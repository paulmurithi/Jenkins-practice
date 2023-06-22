pipeline{
    agent any
    stages{
        stage("Clone"){
            steps{
                sh "echo cloning"
                git 'https://github.com/paulmurithi/Jenkins-practice.git'
            }
        }
        stage("build"){
            steps{
                sh "echo building"
            }
        }
        stage("Test"){
            steps{
                sh "echo Testing"
            }
        }
    }
}