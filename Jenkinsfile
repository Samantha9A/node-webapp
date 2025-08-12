    pipeline {
        agent any

        stages {
            stage('Checkout Code') {
                steps {
                    git branch: 'main'
                        credentialsId: 'ded5b590-2f40-410e-ad62-019f62f34202'
                        url: 'https://github.com/Samantha9A/node-webapp'
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
                    bat echo 'Deployment logic goes here'
                }
            }
        }
    }
