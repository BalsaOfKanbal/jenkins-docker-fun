pipeline {
    agent {
        docker {
            image 'centos'
            label 'generic'
            args '-u 0:0 -v /home/jenkins/.ssh:/root/ssh'
        }
    }
    stages {
        stage("Prepare environment") {
            steps {
                sh """
                set +x
            cp -r /root/ssh /root/.ssh
            chown -R root.root /root/.ssh

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
