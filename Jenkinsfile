pipeline {
  agent {
    docker 'python:3.6.1'
  }
  stages {
    stage('Install dependencies') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
    stage('Test') {
      steps {
        sh 'python --version'
      }
    }
  }
}
