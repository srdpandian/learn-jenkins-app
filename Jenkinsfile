pipeline{
    agent any
    tools{
        nodejs 'Node18'
    }
    stages{
        
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