pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
            }
        }
        stage('Tests') {
            steps {
                echo 'Running tests...'
            }
        }        
        stage('Staging') {
            steps {
                echo 'Deploy to staging...'
            }
        }        
        stage('Production') {
            steps {
                echo 'Deploy to production...'
            }
        }                
    }
}
