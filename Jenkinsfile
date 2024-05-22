pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                script {
                    // Desplegar usando http-server
                    sh 'php -S localhost:8000 .'
                }
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}

