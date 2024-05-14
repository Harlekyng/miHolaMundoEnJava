pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Compilando HolaMundo.java...'
                bat 'javac HolaMundo.java'
            }
        }
        stage('Run') {
            steps {
                echo 'Ejecutando HolaMundo...'
                bat 'java HolaMundo'
            }
        }
    }
    post {
        success {
            echo 'El proceso ha finalizado exitosamente.'
        }
        failure {
            echo 'El proceso ha fallado. Verificar los logs para más detalles.'
        }
    }
}