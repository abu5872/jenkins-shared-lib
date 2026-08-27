pipeline {
    agent any

    stages {
        stage('Docker Login') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'dockerhub-credentials', usernameVariable: 'DOCKER_USER', passwordVariable: 'DOCKER_PASS')]) {
                    sh 'echo "$DOCKER_PASS" | docker login -u "$DOCKER_USER" --password-stdin'
                }
            }
        }
        
        stage('Build and Push') {
            steps {
                script {
                    echo "Building and pushing Docker image..."
                    // Yahan aap apna docker build aur push ka command likh sakte hain
                }
            }
        }
    }
}
