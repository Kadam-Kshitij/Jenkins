pipeline {
    agent {
        docker { image 'ubuntu:20.04' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo $PWD'
                sh 'df -h'
                sh 'ls /home'
                sh 'which gcc'
            }
        }
    }
}
