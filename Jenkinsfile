pipeline {
    agent any

    stages {
        stage('Stage 1') {
            steps {
                git branch: 'main', url:'https://github.com/RaupeCHR/jenkins-python.git'
            }
        }
        stage('Stage 2') {
            steps {
                sh 'python3 main.py'
            }
        }
        stage('Test-Stage') {
            steps {
                sh 'python3 test.py'
            }
        }
    }
}
