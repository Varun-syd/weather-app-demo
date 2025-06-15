pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo '🔄 Pulling code from GitHub...'
            }
        }
        stage('Build') {
            steps {
                echo '⚙️ Running build step...'
                sh 'ls -l'
            }
        }
        stage('Docker Build') {
            steps {
                echo '🐳 Building Docker image...'
                sh 'docker build -t weather-app:latest .'
            }
        }
        stage('Docker Run') {
    steps {
        echo '🚀 Running Docker container...'
        sh 'docker run -d -p 8081:80 --name weather-container weather-app:latest'
    }
}
}
}
      
