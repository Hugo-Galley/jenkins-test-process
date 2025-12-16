pipeline {
  agent {
    docker {
      image 'python:3.14'
    }

  }
  stages {
    stage('Build') {
      steps {
        git(branch: 'main', url: 'https://github.com/Hugo-Galley/jenkins-test-process')
        sh 'python main.py'
      }
    }

  }
}