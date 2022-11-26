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
        stage('Deploy') {
            steps {
                sh 'cp ./exe /home/kshitij/JenkinsBuild'
            }
        }
    }
    post { 
        cleanup { 
            sh 'echo $PWD'
            sh 'ls'
        }
    }
}
