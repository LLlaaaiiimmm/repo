pipeline {
    agent any

    stages {
        stage('Conditional deploy') {
            when {
                expression { return fileExists ('prod.go') }
            }
            steps {
                sh 'chmod +x deploy.sh'
                sh './deploy.sh'
            }
        }
    }
}
