pipeline {
    agent any
    stages {
        stage('CleanWS') {
            steps {
                cleanWS()
            }
        }
        stage('Checkout Git') {
            steps {
                git branch: 'main', credentialsId: 'Github', url: 'https://github.com/Ramlu/mrdevops_java_app.git'
            }
        }
}
}