pipeline {
    agent any

    environment {
        GIT_CREDENTIALS = credentials('github-pat')  // Use ID of your secret text credential
    }

    stages {
        stage('Clone Git Repo') {
            steps {
                git url: "https://${GIT_CREDENTIALS}@github.com/nandhab/eks-example.git", branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo 'Pretend we are building the project...'
            }
        }
    }
}
