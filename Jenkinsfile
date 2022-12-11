pipeline {
    agent any
    environment {
        ENV_URL = "pipeline.jenkins.io"
        SSH_CRED = credentials('SSH')
    }

    stages {

        stage('lint checks') {    //This is to perform lint checks
            steps {
                sh "echo Performing lint checks"
            }
        }  

        stage('Main') {
            when { branch 'main'}
            steps {
                sh "echo"
                sh " echo I am main branch"
            }
        }

    }
}


// SSH_CRED_USR
// SSH_CRED_PSW
