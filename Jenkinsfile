pipeline {
    agent {
        label "jenkins-agent"
    }

    tools {
        maven 'Maven3'
        jdk 'Java17' 
    }

    stages {
        stage("Cleanup Workspace") {
            steps {
                cleanWs() 
            }
        }
        
    }
    stages {
        stage("Checkout from SCM") {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/tusharsense/complete-prodcution-e2e-pipeline' 
            }
        }
        
    }
}