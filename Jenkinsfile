node {
    stage('SCM') {
     git 'https://github.com/skatta3/AWS-JavaProject.git' 
    }
     stage('Maven') {
        sh 'mvn package'       
    }  
   stage('Archive') {
    archiveArtifacts artifacts: 'target\\messageUtil-1.0.jar', followSymlinks: false    
    }
    
}
