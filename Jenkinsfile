pipeline {
    agent any

    tools {
        maven 'maven'
    }

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/ErkkilaT/AuctionBackend', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}