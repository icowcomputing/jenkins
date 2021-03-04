pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo ${ENV, var="$GIT_BRANCH"}
            }
        }
    }
}
