pipeline {
    agent any
    stages {
        stage('Run 04.06.sh') {
            steps {
                script {
                    def currentDate = new Date().format('MM-dd')
                    def filename = '04.06.sh'
                    if (currentDate == filename.replaceAll('.sh', '')) {
                        sh "cat $filename"
                    } else {
                        sh 'chmod +x ./$filename'
                        sh "./$filename"
                    }
                }
            }
        }
        stage('Run 10.10.sh') {
            steps {
                script {
                    def currentDate = new Date().format('MM-dd')
                    def filename = '10.10.sh'
                    if (currentDate == filename.replaceAll('.sh', '')) {
                        sh "cat $filename"
                    } else {
                        sh 'chmod +x ./$filename'
                        sh "./$filename"
                    }
                }
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
