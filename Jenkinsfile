pipeline {
    agent any

    stages {

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


