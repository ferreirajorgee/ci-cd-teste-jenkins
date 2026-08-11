pipeline {
    agent any

    stages {
        stage('Instalação das dependências') {
            steps {
                sh 'npm install'
            }
        }

        stage('Execução dos testes') {
            steps {
                sh 'npm test'
            }
        }
    }
}