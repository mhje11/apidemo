pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/mhje11/apidemo.git', credentialsId: 'mhje11 _github_id'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                 sh 'chmod 755 ./gradlew'
                 sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // test steps
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // deploy steps
            }
        }
    }
}