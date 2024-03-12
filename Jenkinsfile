pipeline {
    // agent any
    agent {
        label "Agent-1"
    }
    stages {
        stage('build') {
            steps {
                echo "Building..."
            }
        }
        stage('test') {
            steps {
                echo "Testing..."
            }
        }
        stage('deploy') {
            steps {
                echo "Deployimg..."
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