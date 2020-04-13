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
                cat /etc/hostname
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
