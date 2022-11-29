pipeline {
    agent any
    stages{
    stage('SCM') {
     git branch: 'release', url: 'https://github.com/skatta3/AWS-JavaProject.git' 
    }
     stage('Maven') {
        sh 'mvn package'       
    }  
   stage('Archive') {
    when{
        branch:'main'
    }
    steps{
    archiveArtifacts artifacts: 'target\\messageUtil-1.0.jar', followSymlinks: false    
    }
   }
    }
    
}

