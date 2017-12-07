pipeline {
    agent any

    environment {
        DISABLE_AUTH = 'true'
        DB_ENGINE    = 'sqlite'
    }

    stages {
        stage('Build') {
            steps {
                sh 'git rev-parse --abbrev-ref HEAD'
                sh 'git branch | grep \* | cut -d ' ' -f2-'
            }
        }
    }
}