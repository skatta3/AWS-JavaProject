pipeline{
    agent any
    stages{
       stage('GetCode'){
            steps{
              git branch: 'Release', url: 'https://github.com/skatta3/AWS-JavaProject.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'
            }
         }
    }
}
