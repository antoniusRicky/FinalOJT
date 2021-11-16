pipeline {
    agent any
    
    stages {
        stage('git repo & clean') {
            steps {
                checkout scm
            }
        }
        stage('install') {
            steps {
                bat "mvn install"
            }
        }
    }
}
