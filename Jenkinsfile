pipeline {
    agent {
        docker {
            image 'python'
            label 'generic'
            
        }
    }
    stages {
        stage("blah") {
            steps {
                sh """
                    python helloworld.py
                """
            }
        }
    }
}
