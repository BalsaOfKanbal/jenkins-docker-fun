pipeline {
    agent {
        docker {
            image 'centos'
            label 'generic'
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
