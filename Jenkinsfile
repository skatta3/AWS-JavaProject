node {
    stage('SCM') {
     git branch: 'Release', url: 'https://github.com/skatta3/AWS-JavaProject.git' 
    }
     stage('Maven') {
        bat 'mvn package'       
    }  
   stage('Archive') {
    archiveArtifacts artifacts: 'target\\messageUtil-1.0.jar', followSymlinks: false    
    }
    
}
