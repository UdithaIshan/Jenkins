pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                    cd /build/
                    cmake ../
                    make
                '''
            }
        }
        stage('Test') {
            steps {
                sh './test'
            }
        }
    }
}