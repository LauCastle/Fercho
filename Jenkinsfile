pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // Instalando dependencias
                    sh 'npm install'
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    // Aquí puedes añadir comandos de construcción si es necesario
                    echo 'Building...'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Desplegar usando http-server
                    sh 'nohup npm start &'
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

