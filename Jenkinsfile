pipeline {
	agent any
    stages {
        stage('Build') {
            sh 'java -version'
            sh 'mvn --version'
            sh 'mvn clean install -Dmaven.test.skip=true'
        }
        stage('Test') {
            sh 'mvn test'
        }
    }
}