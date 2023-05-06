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
                    sh "ssh -tt ubuntu@44.204.72.158"
                    sh "mkdir basha"
                }
            }
        }
    }
}
