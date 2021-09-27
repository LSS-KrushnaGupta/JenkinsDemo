pipeline {
    agent any
    stages {
        stage('Deploy') {
            when { tag "RC-*" }
            steps {
                echo 'Deploying only because this commit is tagged...'
                sh 'make deploy'
            }
        }
    }
}
