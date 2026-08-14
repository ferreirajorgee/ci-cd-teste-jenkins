pipeline {
    agent any

    tools {
        nodejs 'nodejs'
    }

    stages {
        stage('Instalação das dependências') {
            steps {
                echo 'Instalando dependências do projeto...'
                bat 'npm install'
            }
        }

        stage('Execução dos testes') {
            steps {
                echo 'Executando testes...'
                bat 'npm test'
            }
        }
    }

    post {
        success {
            echo 'Build e testes concluídos com sucesso!'
        }
        failure {
            echo 'Falha na execução do pipeline.'
        }
    }
}