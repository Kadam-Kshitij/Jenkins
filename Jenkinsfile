    pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'g++-10 -o exe Hello.cpp'
                sh './exe'
            }
        }
        stage('Clean') {
            echo pwd
        }
    }
}
