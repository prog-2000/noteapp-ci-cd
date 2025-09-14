pipeline{
    agent any
    
    stages{
        stage("Code clone"){
            steps{
                echo "Cloning the code"
                get url: "https://github.com/prog-2000/noteapp-ci-cd.git", branch: "main"
            }
        }
        stage("Code Build"){
            steps{
                echo "Building the image"
                sh "docker build -t my-node-app ."
            }
        }
        stage("Push to DockerHub"){
            steps{
                echo "Push code on dockerhub"
            }
        }
        stage("Deploy"){
            steps{
                echo "Deploy the code"
            }
        }
        
    }
}
