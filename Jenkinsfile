pipeline {
    agent { label 'agent3' }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/FERXX0/Jenkins_Go.git'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./... -v -json > result.json'
            }
        }
    }


}
