pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Check out the source code from your version control system
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                // Run your build commands, e.g., Maven or Gradle
                sh 'mvn clean install'
            }
        }
        
        stage('Test') {
            steps {
                // Run your test commands
                sh 'mvn test'
            }
        }
    }
    
    post {
        always {
            // Clean up or post-processing steps
        }
    }
}
