pipeline {
    agent any

    stages {

        stage('Checkout GitHub') {
            steps {
                git 'https://github.com/shreyasinha2023a-pixel/movie-rating-app.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t movie-rating-app .'
            }
        }

        stage('Run Application') {
            steps {
                sh 'docker run movie-rating-app'
            }
        }
    }
}