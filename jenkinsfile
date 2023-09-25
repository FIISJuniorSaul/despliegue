pipeline {
    agent any

    stages 
    {
        stage('Build') {
            steps {
                echo 'Build app'
            }
        }
        stage('Test') {
            steps {
                echo 'Test app'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy app'
            }
        }
    }
    post
    {
        failure
        {
            emailext body: 'sumary', subject: 'estado pipeline', to: 'junior.saul.maiz@gmail.com'
        }
    }
}
