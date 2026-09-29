pipeline {
    agent any

    stages {

        stage('Check') {
            steps {
                bat 'echo Hello from Jenkins'
            }
        }

        stage('Build') {
            steps {
                bat 'flutter --version'
                bat 'flutter pub get'
                bat 'flutter build apk'
            }
        }

        stage('Test') {
            steps {
                bat 'flutter test'
            }
        }
    }
}