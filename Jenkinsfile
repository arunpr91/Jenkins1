pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your code from version control, for example Git
                git 'https://github.com/arunpr91/Jenkins1.git'
            }
        }
        stage('Build') {
            steps {
                // Run Maven build
                bat 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Run Maven tests
                bat 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Run Maven package or deploy to your repository
                // Modify this according to your project needs
                bat 'mvn package'
            }
        }
    }
}
