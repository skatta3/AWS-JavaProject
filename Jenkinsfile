node {
    stage('SCM') {
     git branch: 'release', url: 'https://github.com/skatta3/AWS-JavaProject.git' 
    }
     stage('Maven') {
        sh 'mvn package'       
    }  
   stage('Archive') {
    when{
        expression{
            env.BRANCH_NAME=='main'
        }
    }
    steps{
    archiveArtifacts artifacts: 'target\\messageUtil-1.0.jar', followSymlinks: false    
    }
   }
    
}

