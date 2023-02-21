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
                    sh 'ssh 172-31-39-165'
                    sh 'mkdir basha'
                }
            }
        }
    }
}
