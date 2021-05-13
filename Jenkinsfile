pipeline {
    agent any 
    environment {
        GITHUB_TOKEN = "Nothing"
    }
    stages {
        stage('Build') {
            steps { 
                sh 'aws cloudformation create-stack --stack-name myteststack --template-body ./cloudformation/emr-jenkins.yml --parameter-overrides $(cat ./cloudformation/parameters/emr.ini)'
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
