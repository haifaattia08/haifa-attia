pipeline {
    agent any
    stages {
        stage('Checkout Git') {
            steps {
                checkout scm
            }
        }
        stage('Build Maven') {
            steps {
                dir('backend') {
                    sh 'mvn clean package -DskipTests'
                }
            }
        }
    }
}


