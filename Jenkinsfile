def projectName = 'compact-disc'
def version = "0.0.${currentBuild.number}"
def dockerImageTag = "${projectName}:${version}"


pipeline {
    agent any

    stages {
        
        stage('Test App') {
            steps {
                echo 'Testing App'
            }
        }
            
        stage('Build Container') {
            steps {
                sh 'docker-compose build'
            }
        }   
            
         stage('Deploy to Openshift ') {
            steps {
                echo 'Deploying to Openshift'
            }
        }
    }
}
