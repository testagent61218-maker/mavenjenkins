pipeline 
{
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building application'
            }
        }
    
        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }
    
        stage('Deploy') {
            steps {
                echo 'Deploying app'
            }
        }
    }
    post {
        always {
            emailext body: 'Summary', subject: 'Pipeline Status', to: 'testagent61218@gmail.com'
        }
    }
}
