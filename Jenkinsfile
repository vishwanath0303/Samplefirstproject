pipeline {
    agent { label "dev-server" }
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/vishwanath0303/Samplefirstproject.git", branch: "main"
            }
        }
        stage("Build and Test"){
            steps{
                sh "docker build . -t node-app-test-new"
            }
        }
        }
    }
}
