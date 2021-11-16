pipeline {
    agent any
    
    stages {
        stage('git repo & clean') {
            steps {
                checkout scm
            }
        }
        stage('build') {
            steps {
                bat "mvn clean package -Dmaven.test.skip=true"
            }
        }
    }
}
