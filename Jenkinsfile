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
                bat 'git config --global --add safe.directory C:/src/flutter_windows_3.47.5-stable/flutter'
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