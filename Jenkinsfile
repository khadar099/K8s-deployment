pipeline {
    
    agent any 
    
    stages {
        stage('Git Checkout') {
            
            steps {
                
                script {
                    
                    git branch: 'main', url: 'https://github.com/khadar099/K8s-deployment.git'
                }
            }
        }
        stage ('deploy app') {
            steps {
                script {
                    //sh 'ssh -tt ubuntu@ip-172-31-39-165 -oStrictHostKeyChecking=no'
                    sh 'ssh -it "key182.pem" ubuntu@ec2-43-207-4-75.ap-northeast-1.compute.amazonaws.com'
                    sh 'mkdir basha'
                }
            }
        }
    }
}
