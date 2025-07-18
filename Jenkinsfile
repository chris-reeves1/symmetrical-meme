pipeline{
    agent any
    stages{
        stage("Make a directory"){
            steps{
                sh "mkdir ~/jenkins || true"
        }
        }                    
        stage("add file"){
            steps{
                sh "touch ~/jenkins/file.txt"
            }
        }



                       
    }
}

