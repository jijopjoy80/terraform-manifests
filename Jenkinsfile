pipeline {
    agent any
    
    environment {
        AWS_ACCESS_KEY_ID = credentials('myawscreds')
        AWS_SECRET_ACCESS_KEY = credentials('myawscreds')
    }

    
    stages {
        stage('Code Checkout') {
            steps {
                git branch: 'master',
                    credentialsId: 'github-jenkins',
                    url: 'https://github.com/jijopjoy80/terraform-manifests.git'
                }
        }

    }     

        
}
