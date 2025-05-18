pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }
            steps {
                sh '''
                    echo "steps start.."
                    ls -la
                    node --version
                    npm --version
                '''
            }
        }
    }
}
