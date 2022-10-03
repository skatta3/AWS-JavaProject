node {
    stage('SCM') {
     git branch: 'main', url: 'https://github.com/skatta3/AWS-JavaProject.git' 
    }
     stage('Maven') {
        sh 'mvn package'       
    }  
   stage('Archive') {
    archiveArtifacts artifacts: 'target\\AWS-JavaProject.war', followSymlinks: false    
    }
    
}