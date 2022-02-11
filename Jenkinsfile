pipeline {
    agent any
    
    stages {
        stage('Build Docker image') {
            steps {
                sh 'docker build -t docker-getting-started .'
            }
        }

        stage('Run Docker Container 3000') {
            steps {
                sh 'docker run -dp 3000:3000 docker-getting-started'
            }
          }
    }
}
