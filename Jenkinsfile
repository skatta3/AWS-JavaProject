node{
    stage('Build'){
        steps{
            script{
                if(env.BRANCH_NAME=='main'){
                    git branch: 'main', url: 'https://github.com/skatta3/AWS-JavaProject.git'
                    sh 'mvn package'
                    archiveArtifacts artifacts: 'target\\messageUtil-1.0.jar', followSymlinks: false
                }
            }
        }
    }
}

