pipeline{
    agent{
        label "jenkins-agent"
    }
    tools {
        maven 'Maven3'
        jdk 'Java17'
        
    }
    stages{
        stage("Cleanup Workspace"){
            steps {
                cleanWs()
            }

        }
    
        stage("Checkout from SCM"){
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/harshitjaiswal394/complete-prodcution-e2e-pipeline.git'
            }

        }
    }
}