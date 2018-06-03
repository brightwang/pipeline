pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('cheif check') {
            steps {
                input message: '是否确定发布到生产环境？', submitter: 'demo'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always {
            echo 'end'
        }
        failure {
            echo 'failure'
        }
    }
}
