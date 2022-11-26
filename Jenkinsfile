pipeline {
    agent {
        docker { image 'ubuntu:20.04' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo $PWD'
                sh 'whoami'
            }
        }
    }
}
