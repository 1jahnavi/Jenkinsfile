pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Build your code here
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Run tests here
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the application
                sh 'deploy.sh'
            }
        }

        stage('Post-Deployment') {
            steps {
                // Perform post-deployment tasks
                sh 'post-deployment.sh'
            }
        }
    }