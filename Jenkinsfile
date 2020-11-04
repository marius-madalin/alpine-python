pipeline {
    agent {
        docker {
            image 'marius25madalin/getting-started:alpine-python'
            args '-v $HOME/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'python dateParser.py'
            }
        }
    }
}
