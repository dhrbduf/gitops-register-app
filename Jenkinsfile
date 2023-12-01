pipeline {
    agent any

    environment {
              APP_NAME = "register-app-pipeline"
    }
    
    stages {
        stage("Cleanup Workspace") {
            steps {
                cleanWs()
            }
        }

        stage("Checkout from SCM") {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/dhrbduf/gitops-register-app'
            }
        }


    }
}
