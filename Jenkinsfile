pipeline {
    agent {
        docker {
            label 'generic'
            image 'centos'
        }
    }
    stages {
        stage("Prepare environment") {
            steps {
                sh """
                yum install python -y
                """
            }
        }
        stage("blah") {
            steps {
                sh """
                    python helloworld.py
                """
            }
        }
    }
}