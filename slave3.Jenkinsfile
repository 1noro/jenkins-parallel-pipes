pipeline {
    agent any
    stages {
        stage('stuff') {
            steps {
                sh 'echo "hello from slave3 (the random one)"'
                sh 'sleep 3'
                sh 'exit $(($RANDOM % 2))'
            }
        }
    }
}
