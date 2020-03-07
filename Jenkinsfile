pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
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
                prompt 'Proceed?'
                echo 'Deploy to production...'
            }
        }                
    }
}
