pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'git@github.com:massicito04/test.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install' // Adapté selon ton projet (mvn, npm, etc.)
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test' // Adapté selon ton projet
            }
        }

    }
}
