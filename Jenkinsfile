pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                        echo "Hello, This is build"
                    """
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh """
                        echo "Hello, This is test"
                    """
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    sh """
                        echo "Hello, This is Deploy"
                    """
                }
            }
        }
    
    }

    post {
        always {
            echo "I will always say Hello again"
        }
        failure {
            echo "I will run when pipeline is failed"
        }
        success {
            echo "I will run when the pipeline is success"
        }
    }
}