pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Application'
            }
        }
        stage('Test') {
            steps {
                echo 'Test Application'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Application'
            }
        }
    }
    post {
        always {
            emailext body: 'Summary', subject: 'Pipeline Status', to: 'www.pooja1407@gmail.com'
        }
    }
}
