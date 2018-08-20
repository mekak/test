# test
properties([pipelineTriggers([githubPush()])])
pipeline{
    agent any
    stages{      
        stage("check out"){
            steps{
               git “https://bitbucket.org/test.git” 
            	}
          }
      }
}
