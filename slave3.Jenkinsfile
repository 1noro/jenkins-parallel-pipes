pipeline {
    agent any
    stages {
        stage('stuff') {
            steps {
                sh '''
                    echo hello from slave3 (the random one)
                    sleep 3
                    exit $(($RANDOM%2))
                '''
            }
        }
    }
}
