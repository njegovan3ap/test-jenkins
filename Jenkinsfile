pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'java -version'
                sh 'mvn --version'
                sh 'mvn clean install -Dmaven.test.skip=true'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}