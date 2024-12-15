pipeline {
    agent any
    stages {
        stage('Deploy to Kubernetes') {
            steps {
                script {
                    sh 'kubectl apply -f namespace.yaml'
                    sh 'kubectl apply -f prometheus-config.yaml'
                    sh 'kubectl apply -f prometheus-deployment.yaml'
                    sh 'kubectl apply -f prometheus-service.yaml'
                    sh 'kubectl apply -f grafana-deployment.yaml'
                    sh 'kubectl apply -f grafana-service.yaml'
                    '''
                }
            }
        }
    }
}
