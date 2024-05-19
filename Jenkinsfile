pipeline {

    agent any 

    environment {
        GIT_BRANCH = 'main'
        GIT_CREDENTIALS = 'Github'
        GIT_URL = 'https://github.com/Ramlu/mrdevops_java_app.git'
    }

    stages {

        stage('Clean WS') {
            steps {
                cleanWs()
            }
        }

        stage('Checkout Git') {
            steps {
                git branch: "${GIT_BRANCH}", credentialsId: "${GIT_CREDENTIALS}", url: "${GIT_URL}"
            }
        }
    }

}