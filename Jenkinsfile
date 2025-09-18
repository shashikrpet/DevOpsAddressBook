pipeline {
    agent any

      stages {
      stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/your-repo/your-project.git'
            }
        }

        stage('Build with Maven') {
            steps {
                sh 'mvn clean install'
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}





















    
