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
}