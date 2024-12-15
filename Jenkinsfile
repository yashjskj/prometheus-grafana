pipeline {
    agent any
    stages {
        stage('Deploy to Kubernetes') {
            steps {
                script {
                    sh 'kubectl apply -f k8s/namespace.yaml'
                    sh 'kubectl apply -f k8s/frontend-deployment.yaml'
                    sh 'kubectl apply -f k8s/frontend-service.yaml'
                    '''
                }
            }
        }
    }
}
