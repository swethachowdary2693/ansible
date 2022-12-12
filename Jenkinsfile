pipeline {
    agent any
    environment {
        ENV_URL = "pipeline.jenkins.io"
        SSH_CRED = credentials('SSH')
    }

    stages {
        
        stage('lint checks') {    //This is to perform lint checks
        when { branch pattern: "feature-.*", comparator: "REGEXP" }    
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

        stage('Tag') {
            when { expression { env.TAG_NAME =! null }}
            steps {
                sh "echo"
                sh "echo Against tag"
            }
        }

    }
}


// SSH_CRED_USR
// SSH_CRED_PSW
