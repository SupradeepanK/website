pipeline {
    agent any

    environment {
        IMAGE_NAME = "website-app"
    }

    stages {

        stage('Build') {
            steps {
                echo "Building Docker Image..."
                sh 'docker build -t $IMAGE_NAME .'
            }
        }

        stage('Test') {
            steps {
                echo "Running Test Container..."
                sh 'docker run -d -p 8081:80 $IMAGE_NAME'
            }
        }

        stage('Deploy to Prod') {
            when {
                branch 'master'
            }
            steps {
                echo "Deploying to Production..."
                sh '''
                docker stop prod-container || true
                docker rm prod-container || true
                docker run -d -p 80:80 --name prod-container $IMAGE_NAME
                '''
            }
        }
    }
}
