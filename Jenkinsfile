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
                sh 'sudo cp -r ./exe /home/kshitij/JenkinsBuild'
            }
        }
    }
    post { 
        cleanup('CleanUp') { 
            sh 'sudo rm -rf /var/lib/jenkins/workspace/*'
        }
    }
}
