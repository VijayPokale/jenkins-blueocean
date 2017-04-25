pipeline {
  agent {
    docker 'python:3.6.1'
  }
  stages {
    stage('Virtualenv') {
      steps {
        sh 'virtualenv --no-site-packages .'
      }
    }
    stage('Install dependencies') {
      steps {
        sh 'source bin/activate && pip install -r requirements.txt && deactivate'
      }
    }
    stage('Test') {
      steps {
        sh 'python --version'
      }
    }
  }
}
