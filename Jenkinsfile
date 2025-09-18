pipeline {
    agent any

      stages {
      stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/shashikrpet/DevOpsAddressBook.git'
            }
        }

        
        stage('Build with Maven') {
            steps {
                sh 'mvn clean package'
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





















    
