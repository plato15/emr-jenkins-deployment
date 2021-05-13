pipeline {
    agent any 
    environment {
        GITHUB_TOKEN = "Nothing"
    }
    stages {
        stage('Build') {
            steps { 
                sh 'echo HI I am Build'
            }
        }
        stage('Test') {
            steps {
                sh 'echo HI I am Test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo HI I am Deploy'
            }
        }
    }
}
