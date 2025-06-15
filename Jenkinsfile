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
        stage('Success') {
            steps {
                echo '✅ Build completed successfully!'
            }
        }
    }
}

