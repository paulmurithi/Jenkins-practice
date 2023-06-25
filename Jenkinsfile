pipeline{
    agent any
    stages{
        stage("Clone"){
            steps{
                echo "cloning..."
                git 'https://github.com/paulmurithi/Jenkins-practice.git'
            }
        }
        stage("build"){
            steps{
                echo "building..."
            }
        }
        stage("Test"){
            steps{
                echo "Testing..."
            }
        }
    }
}