pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: ' https://github.com/Ritabrata123github/Jenkins_demo '
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p ~/deploy-demo
                cp index.html ~/deploy-demo/
                '''
            }
        }
    }
}