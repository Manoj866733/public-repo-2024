pipeline {

    agent any

    tools {
        maven 'Maven3'
    }

    stages {

        stage('Git Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Manoj866733/public-repo-2024.git']])
            }
        }
        stage('Git Checkout') {
            steps {
                sh 'mvn clean install -f pom.xml'
            }
        }
    }
}
