pipeline{
    agent any
    stages{
        stage("Make a directory"){
            steps{
                script(catchError(buildResult: "UNSTABLE", stageResult: "UNSTABLE"){
                sh "mkdir ~/jenkins"
                }
            }
        }
        }
        stage("add file"){
            steps{
                sh "touch ~/jenkins/file.txt"
            }
        }

    }
}

