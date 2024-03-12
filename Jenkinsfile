pipeline {
    // agent any
    agent {
        label "Agent-1"
    }
    stages {
        stage('build') {
            steps {
                echo "Building..." // echo command only will run directly...other linux commands must mention in sh ''
                // running linux coomand
                sh 'ls -ltr'
                sh 'pwd'
                sh 'date'

            }
        }
        stage('test') {
            steps {
                echo "Testing..."
                 sh 'hostname -f'
                sh 'uname'
            }
        }
        stage('deploy') {
            steps {
                echo "Deployimg..."
                // we can mention multiple linux commands like bellow ('''')
                sh '''    
                df -h
                free -m
                '''
                echo "PESI"
            }
        }
    }
    post {
        always {
            echo "Always do this when pipeline triggered"
        }
        success {
            echo "Run at the time of SUCCESS"
        }
        failure {
            echo "Run at the time of failure"
        }
    }
}