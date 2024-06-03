pipeline {
    agent any
    stages {
        stage('Run test1.sh') {
            steps {
                sh 'chmod +x ./test1.sh'
                sh './test1.sh'
            }
        }
        stage('Run test2.sh') {
            steps {
                sh 'chmod +x ./test2.sh'
                sh './test2.sh'
            }
        }
        stage('Run test3.sh') {
            steps {
                sh 'chmod +x ./test3.sh'
                sh './test3.sh'
            }
        }
    }
    post {
        success {
            echo 'Pipeline execution successful!'
        }
        failure {
            echo 'Pipeline execution failed :('
        }
    }
}
