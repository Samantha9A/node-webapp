    pipeline {
        agent any

        stages {
            stage('Checkout') {
                steps {
                    git branch: 'main'
                        credentialsId: 'ded5b590-2f40-410e-ad62-019f62f34202'
                        url: 'git@github.com:Samantha9A/node-webapp.git'
                }
            }
            stage('Build') {
                steps {
                    sh 'npm install'
                }
            }
            stage('Test') {
                steps {
                    sh 'npm test'
                }
            }
            stage('Deploy') {
                steps {
                    echo 'Deployment logic goes here'
                }
            }
        }
    }
