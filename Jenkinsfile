pipeline {
    agent any

    stages {

        stage('Inicio') {
            steps {
                echo 'INICIO DEL PIPELINE'
            }
        }

        stage('Verificar Git') {
            steps {
                sh 'git --version'
            }
        }

        stage('Verificar Repositorio') {
            steps {
                sh 'ls -la'
            }
        }

        stage('Finalizacion') {
            steps {
                echo 'PIPELINE EJECUTADO CORRECTAMENTE'
            }
        }
    }
}