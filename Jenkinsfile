pipeline {
    agent any
    stages {
        stage('Checkout Main Repo') {
            steps {
                git 'https://github.com/AhmedSaid25/cloud-task-bash.git'
            }
        }
        stage('Clone Secondary Repo') {
            steps {
                sh 'git clone https://github.com/AhmedSaid25/cloud-task-bonus.git secondary-repo'
            }
        }
        stage('Execute Script on Secondary Repo') {
            steps {
                dir('secondary-repo') {
                    sh 'bash ../script.sh'
                }
            }
        }
    }
}
