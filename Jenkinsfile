pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                ${ENV, var="$GIT_BRANCH"}
                echo ${var}
            }
        }
    }
}
