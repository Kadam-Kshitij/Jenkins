    pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                g++-10 -o exe Hello.cpp
                ./exe
            }
        }
        stage('Clean') {
            echo pwd
        }
    }
}
