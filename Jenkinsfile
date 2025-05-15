pipeline {
    agent any
    environment {
        PATH = "/opt/homebrew/bin:$PATH"
    }
    stages {
        stage('Check Minikube') {
            steps {
                sh 'minikube status'
            }
        }
        stage('Get K8s Nodes') {
            steps {
                sh 'kubectl get nodes'
            }
        }
    }
}