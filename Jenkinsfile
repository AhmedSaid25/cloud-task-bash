pipeline {
    agent any
    stages {
        stage('Clone and List Files') {
            steps {
                script {
                    // Clean up workspace to avoid conflicts
                    // deleteDir()

                    // Clone the second repository
                    git url: 'https://github.com/AhmedSaid25/cloud-task-bonus.git', branch: 'main'

                    // List the files in the cloned repository
                    bat 'dir'
                }
            }
        }
    }
}