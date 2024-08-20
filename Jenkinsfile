pipeline {
    agent any

    stages {
        stage('build') {
            docker {
                image 'node:18-apline'
                reuseNode true
            }
        }
        steps{
            sh '''
                ls -la
                node --version
                npm --version
                npm cli
                npm run build
                ls -la
            '''
        }
    }
}