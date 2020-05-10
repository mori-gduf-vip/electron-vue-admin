pipeline {
    agent {
        docker { image 'node:latest' }
    }
     stages {
            stage('Build') {
                steps {
                    sh 'node --version'
                    echo 'Building..'
                    sh 'npm install'
                    echo 'packing..'
                    sh 'npm run pack'
                    echo 'build..'
                    sh 'npm run build'

                }
            }
            stage('Test') {
                steps {
                    echo 'Testing..something'
                }
            }
            stage('Deploy') {
                steps {
                    echo 'Deploying....'
                }
            }

        }
}