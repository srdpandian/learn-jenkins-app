pipeline{
    agent any
    stages{
        tools {
            nodejs 'Node18'
        }
        stage('Build'){
            steps{
                sh '''
                    ls -la
                    node --version
                    npm --version
                    npm ci
                    npm run build
                    ls -la
                '''
            }
            
        }
    }
}