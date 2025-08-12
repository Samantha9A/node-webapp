    pipeline {
        agent any

        environment {
        DOCKER_IMAGE = 'sidharthsingh7/ss_backend'
        DOCKER_TAG = "0.0.1.RELEASE"
        }
        stages {
            stage('Checkout Code') {
                steps {
                    git 'https://github.com/Samantha9A/node-webapp'
                }
            }
            stage('Build') {
                steps {
                    bat 'echo "Building the app"'
                }
            }
            stage('Test') {
                steps {
                    bat 'echo "Running tests"'
                }
            }
            stage('Deploy') {
                steps {
                    bat 'echo "Deployment logic goes here"'
                }
            }
        }
    }
