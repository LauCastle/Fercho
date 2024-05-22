pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                script {
                    // Desplegar usando http-server
                    bat 'php.exe --version'
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

