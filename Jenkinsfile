pipeline {
    agent any
    stages {
        stage('Deploy to Kubernetes') {
            steps {
                script {
                    sh '''
                    kubectl apply -f namespace.yaml
                    kubectl apply -f prometheus-config.yaml
                    kubectl apply -f prometheus-deployment.yaml
                    kubectl apply -f prometheus-service.yaml
                    kubectl apply -f grafana-deployment.yaml
                    kubectl apply -f grafana-service.yaml
                    '''
                }
            }
        }
    }
}