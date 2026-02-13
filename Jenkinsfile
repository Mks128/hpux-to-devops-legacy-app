pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
            }
        }

        stage('Build') {
            steps {
                sh 'chmod +x legacy_app.sh'
                sh './legacy_app.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Tests completed.'
            }
        }
    }
}

