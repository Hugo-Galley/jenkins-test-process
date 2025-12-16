pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/Hugo-Galley/jenkins-test-process'
                
                // Run Python
                sh "python main.py"
            }
        }
    }
}
