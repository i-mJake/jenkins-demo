pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/i-mJake/jenkins-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Run App') {
            steps {
                sh 'node app.js'
            }
        }

        stage('Success Message') {
            steps {
                echo "CI/CD Pipeline executed successfully!"
            }
        }

    }
}