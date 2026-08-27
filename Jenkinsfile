@Library('sharedLib') _

pipeline {
    agent any

    stages {
        stage('Docker Login') {
            steps {
                dockerLogin('dockerhub-credentials')
            }
        }
        
        stage('Build and Push') {
            steps {
                script {
                    echo "Building and pushing Docker image..."
                    // Yahan aap apna docker build aur push ka code likh sakte hain
                }
            }
        }
    }
}
