pipeline {
    agent any
    stages {

        stage('Passos para o MASTER') {
            when { anyOf { branch 'master' } }
            steps {
                sh "echo MASTER"
                sh "php --version"
            }
        }

        stage('Passos para o FEATURE-1') {
            when { anyOf { branch 'feature-1' } }
            steps {
                sh "echo FEATURE-1"
            }
        }

        stage('Passos para os dois BRANCHES') {
            steps {
                sh "echo MASTER e FEATURE"
            }
        }
    }
}
