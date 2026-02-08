pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
               bat 'npm install'
            }
        }
        stage('Run npm security audit') {
            steps {
                bat 'npm run audit'
            }
        }
        stage('Run UI Tests') {
            steps {
                bat 'npm test'
            }
        }
      
    }
}

