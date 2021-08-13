pipeline {
    agent any

    stages {
        
        stage('Build') {
            steps {
                git 'https://github.com/douglasslima/mywebsite-docker.git'
            }
        }
        
        stage('Deploy') {
            steps {
                ansiblePlaybook disableHostKeyChecking: true, installation: 'ansible', playbook: 'deploy-docker.yml'
            }
        }
    }
}

