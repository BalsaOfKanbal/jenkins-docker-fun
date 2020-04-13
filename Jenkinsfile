pipeline {
    agent {
        label 'generic'
    }
    stages {
        stage("blah") {
            steps {
                sh """
                    docker build .
                """
            }
        }
    }
}