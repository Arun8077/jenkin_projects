pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout main and track origin/main
                git branch: 'main', 
                    url: 'https://github.com/Arun8077/jenkin_projects.git', 
                    credentialsId: 'github-creds'
            }
        }

        stage('Confirm') {
            steps {
                // Run git command in workspace
                sh 'git status'
                sh 'git branch --show-current'
            }
        }
    }
}
