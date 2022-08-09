pipeline {
    agent any
    stages {
        stage('printenv') {
            steps {
                sh 'printenv'
            }
        }
        stage ('Run slave1') {
            steps {
                build job: 'parallel-slave1'
            }
        }
        stage ('Run slave2') {
            steps {
                build job: 'parallel-slave2'
            }
        }
        stage ('Run slave3') {
            steps {
                build job: 'parallel-slave3'
            }
        }
    }
}
