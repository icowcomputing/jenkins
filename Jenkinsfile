pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo "${GIT_BRANCH}"
            }
        }
        stage('Docker Build') {
            steps {
                sh 'sudo docker images -a'
                sh 'cd /home/frankie/dev'
                sh 'sudo docker build -t jenkinsapp01 .'
                sh 'sudo docker images -a'
            }
        }
        
    }
}
