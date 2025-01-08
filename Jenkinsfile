pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh './deploy.sh'
            }
        }
        stage('Test') {
            steps {
                sh 'curl -f http://localhost:5000 || exit 1'
            }
        }
    }
}
