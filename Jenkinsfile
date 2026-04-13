pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t movie-rating-app .'
            }
        }

        stage('Run Application') {
            steps {
                bat 'docker run movie-rating-app'
            }
        }
    }
}

