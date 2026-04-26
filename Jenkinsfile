pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Код GitHub-тан алынды'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build басталды'
                sh 'echo Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Тест жүргізілуде'
                sh 'echo Testing...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy орындалды'
                sh 'echo Deploying...'
            }
        }
    }

    post {
        success {
            echo 'SUCCESS ✅'
        }
        failure {
            echo 'ERROR ❌'
        }
    }
}
