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
                bat 'git --version'
            }
        }

        stage('Verificar Repositorio') {
            steps {
                bat 'dir'
            }
        }

        stage('Finalizacion') {
            steps {
                echo 'PIPELINE EJECUTADO CORRECTAMENTE'
            }
        }
    }
}