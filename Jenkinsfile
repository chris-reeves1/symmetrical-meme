// global variables
// persistant
// Used in the groovy script

pipeline{
    agent any
    //environment{ Variables to be passed to sh. creds/paths}
    /*options{
        timestamps() //global
        disableConcurrentBuilds() //global
        timeOut(time: 10, unit: "minutes") //global/local
        retry(5) //stage
    }
    */
    stages{
        stage("Make a directory"){
            catchError(buildResult: "UNSTABLE", stageResult: "UNSTABLE")
            //options{
            //AllowFailure true
            //timeOut(time: 1, units: "minutes")}
            steps{
                sh "mkdir ~/jenkins"
            }
            post {
                success {echo "successful stage!"}
                failure {echo "failed"}
                always{echo "always prints!"}
                /*archivetheartifacts
                email
                clean up actions
                printing file sys
                */ 
            }
        }
        stage("add file"){
            steps{
                sh "touch ~/jenkins/file.txt"
            }
        }
    }
}
