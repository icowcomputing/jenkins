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
                sh 'docker images -a'
                sh 'cd /home/frankie/dev && docker build -t jenkinsapp01 .'
                sh 'docker images -a'
            }
        }
        
    }
}
